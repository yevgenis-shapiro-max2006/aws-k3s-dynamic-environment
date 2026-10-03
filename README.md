<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/15ecd51a-ffdd-49a7-83d0-2edb6b5020fa" />



## AWS | K3S Dynamic Environment
K3s as a lightweight and certified Kubernetes distribution developed by Rancher Labs (now part of SUSE). Designed to streamline deployments in edge computing, IoT, and local development scenarios, K3s provides a simplified alternative to traditional Kubernetes. By consolidating essential components into a single, efficient binary, K3s aims to maintain core Kubernetes functionalities while reducing the overhead typically associated with deployment and management.


🎯  Installation and Integration
```
✅ GitLab — source code, Terraform, Kubernetes manifests
✅ Terraform + reusable Terraform Modules
✅ AWS infrastructure / VM / networking / load balancers
✅ K3s / Kubernetes
✅ Velero + Velero UI — backup and restore
✅ Argo Events / Event-driven GitOps
✅ Kubernetes workloads and resources
```

🚀 
```
terraform init
terraform validate
terraform plan -var-file="template.tfvars"
terraform apply -var-file="template.tfvars" -auto-approve

terraform -chdir=./modules/argo init
terraform -chdir=./modules/argo apply -auto-approve
```

🧩 Config 

```
scp -i ~/.ssh/<your pem file> <your pem file> ec2-user@<terraform instance public ip>:/home/ec2-user
chmod 400 <your pem file>
```

