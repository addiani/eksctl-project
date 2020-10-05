# install aws cli first for linux :
aws --version
pip3 install --upgrade --user awscli ( in case you get an error  pip3 command not found: run sudo yum install python37)
pip --version
aws --version

# configure your aws cli credentials:
aws configre (put your access key and secret key by creating a new user called awscli or different name!)
cat ~/.aws/credeantials

# install eksctl:
curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
sudo mv /tmp/eksctl /usr/local/bin
eksctl version

# Install and configure kubectl:
curl -o kubectl https://amazon-eks.s3.us-west-2.amazonaws.com/1.17.9/2020-08-04/bin/linux/amd64/kubectl
chmod +x ./kubectl
sudo mv ./kubectl /usr/local/bin

# creating the nodes:
# Managed nodes – Linux ]
 eksctl create cluster --name first-eks --region us-east-2 --nodegroup-name standard-nodes --node-type t3.small --managed
which eksctl
which kubectl
ls .kube
kubectl run nginx --image nginx --replicas 2
kubectl get all


# or Launch a Template: lcreate a file call it cluster-eks.yaml:
---
