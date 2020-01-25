# k8s tips

## Clean up evected pods
```
kubectl get pods | grep Evicted | awk '{print $1}' | xargs kubectl delete pod
```

## K8s Structured Logging
https://github.com/kubernetes/enhancements/pull/1367/files#diff-3aa8edd896257b5b538d386cf36727f4

## kubectl Tips
https://itnext.io/boosting-your-kubectl-productivity-b348f7c25712

## Remove Zombie Namespaces
https://www.ibm.com/support/knowledgecenter/en/SSBS6K_3.1.1/troubleshoot/ns_terminating.html

## Install golang
```
sudo apt-get update

sudo apt-get install -y libssl-dev libffi-dev
sudo apt-get install -y python-dev

cd /tmp
wget https://dl.google.com/go/go1.13.6.linux-amd64.tar.gz
sudo tar -xvf go1.13.6.linux-amd64.tar.gz
sudo mv go /usr/local

export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export PATH=$PATH:$GOPATH/bin:$GOROOT/bin

source ~/.profile
source ~/.bashrc
```
