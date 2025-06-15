# Kubernetes Security Scan using Kubescape

## 📌 Problem Statement
Scan a local Kubernetes cluster for security vulnerabilities and provide a report in JSON format.

## 🛠 Tools Used
- Minikube (for local K8s cluster)
- Kubescape (security scanner)

## ✅ Steps Followed
1. Installed Minikube and started a local cluster:
   ```bash
   minikube start
   
2. Installed Kubescape:
   curl -s https://raw.githubusercontent.com/kubescape/kubescape/master/install.sh | /bin/bash
3. Ran the security scan and saved the results in JSON format:
   kubescape scan --submit=false --format json --output kubescape-results.json
