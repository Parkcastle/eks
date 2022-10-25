## terraform eks
EKS configuration using terraform

## install terraform 
- `git clone https://github.com/Parkcastle/marketboro.git`
- `cd ./tf_eks`
- `terraform init`
- `terraform apply -auto-approve`

## Run locally 
- `aws configure --profile user1`
- `aws eks update-kubeconfig --region ap-northeast-2 --name castle-eks --profile eks-admin`
- `echo -e "role_arn = arn:aws:iam::<aws account id>:role/eks-admin\\nsource_profile = user1" >> ~/.aws/config`
- `kubectl get nodes -n kube-system`
