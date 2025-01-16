# eks-iac-terraform
Terraform infraestructure to provisioning EKS Cluster

1. Set up Infrastructure

```bash
cd terraform
terraform init
terraform apply
```

2. Deploy Application
```bash
# Create the Ingress Controller
kubectl create -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.12.0/deploy/static/provider/aws/deploy.yaml
# Apply configurations
kubectl apply -f <your-k8s-configuration-file>
``
