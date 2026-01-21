# Umma Hafsa Himi
### DevOps Practitioner | Operational Engineer | Technical Project Manager
## Resume
[Download Resume](20260119-DevOps-Resume-Himi.pdf)
## Contact
- **Email:** ummahafsahimi@gmail.com
- **Phone:** +1 236-777-4457 
- **LinkedIn:** linkedin.com/in/umma-hafsa-himi/  
- **GitLab Projects:** https://gitlab.com/my-capstone-projects-devops



Hi, I'm a DevOps Engineer who loves turning manual processes into automated solutions. I work with AWS, Kubernetes, Terraform, and Jenkins to build reliable infrastructure that scales.  
Browse my projects to see how I approach real-world DevOps challenges.


## Kubernetes CI/CD Capstone Project: AWS EKS & ECR Integration

Built a production-grade CI/CD pipeline using Jenkins that automates the entire deployment workflow—from code commit to Kubernetes cluster deployment. The pipeline automatically increments versions, builds Java Maven artifacts, creates Docker images, pushes to AWS ECR, deploys to EKS clusters, and commits version updates back to Git for complete version control.

[View Project Repository →](#)

**Pipeline Workflow:**

Automated the complete deployment cycle: increment application version → build Java Maven artifact → create Docker image → push to AWS Elastic Container Registry → deploy to EKS cluster → commit version update to Git. Every step is triggered automatically with proper error handling and rollback capabilities.

**Technologies:** Kubernetes (EKS) • Jenkins (Pipeline-as-Code) • AWS ECR • Java/Maven • Docker • Git • Linux

**Key Learnings:** Created and configured AWS Elastic Container Registry with secure Jenkins authentication using AWS credentials, automated Kubernetes deployments to EKS clusters directly from CI/CD pipelines, applied GitOps principles by maintaining version control throughout the deployment process, and understood how container registries integrate with orchestration platforms for seamless deployments.

**The Result:** A complete DevOps workflow where code changes trigger automated builds, containerization, registry management, and orchestrated deployments—all with zero manual intervention. This demonstrates production-ready CI/CD practices that reduce deployment time from hours to minutes while improving reliability.


## AWS EKS Production Deployment: Stateful & Stateless Applications

Automated deployment of a complete application stack to AWS EKS—combining stateless Java applications with stateful databases in a production-grade Kubernetes environment. Implemented cost optimization through autoscaling and strategic resource allocation across EC2 and Fargate.

[View Project Repository →](https://gitlab.com/my-capstone-projects-devops/aws-a-java-maven-app-deploy-to-eks-cluster.git)

**Architecture:**

Provisioned an AWS EKS cluster using kubectl with 3 EC2 worker nodes and 1 Fargate profile for workload separation. Deployed stateful applications (MySQL and phpMyAdmin) to EC2 nodes using Helm charts with Persistent Volume Claims for data persistence. Deployed the stateless Java Maven application on Fargate with 3 replicas for high availability and cost efficiency.

Integrated AWS ECR as the container registry and built a Jenkins CI/CD pipeline to automate the entire deployment workflow. Configured Kubernetes Horizontal Pod Autoscaler (min=1, regular=2, max=3) to dynamically scale based on load while optimizing costs.

**Technologies:** AWS EKS & ECR • Kubernetes • Docker • Helm • Jenkins • Java/Maven • MySQL • Fargate • Linux • Git

**Key Learnings:** Understood the differences between stateful and stateless application deployment strategies in Kubernetes, configured Persistent Volume Claims for database data persistence, leveraged AWS Fargate for serverless container execution, implemented Helm charts for repeatable deployments, configured Horizontal Pod Autoscaler for cost-effective scaling, and automated multi-component deployments through CI/CD pipelines.

**The Result:** A production-ready Kubernetes deployment that balances performance, reliability, and cost—automatically scaling resources based on demand while maintaining data persistence for stateful workloads. This demonstrates real-world cloud-native architecture patterns.



## Python Automation: Website Monitoring and Self-Healing Recovery

Built an intelligent monitoring system using Python that continuously checks application health, detects failures, and automatically remediates issues without manual intervention. The script monitors a web application running on a Linode server, sends email alerts when problems are detected, and performs self-healing operations like container restarts to restore service.

**Key Features:**
- Continuous health monitoring of application endpoints
- Automated email notifications on server connection failures using SMTPLIB
- Self-healing capability—automatically restarts containers when issues are detected
- Environment variable management for secure credential handling

**Technologies:** Python • Linode • Docker • Nginx • Linux • SMTPLIB • Environment Variables

**Key Learnings:** Provisioned and configured Linode servers with SSH access, deployed containerized applications with Docker, implemented Gmail SMTP authentication for automated alerting, configured environment variables for secure credential management, and built proactive monitoring that reduces downtime through automated recovery.

This project demonstrates SRE principles of reducing toil and improving reliability—transforming reactive incident response into proactive, automated problem resolution.

[View Project Repository →](#)

## Ansible Capstone Project: Orchestrating Cloud Infrastructure with Code

Solved the real-world challenge of provisioning cloud infrastructure and deploying applications in a fully automated, repeatable way—everything defined as code, version-controlled, and executable with a single command.

[View Project Repository →](https://gitlab.com/my-capstone-projects-devops/ansible-demo-deploy-application-to-kubernetes-eks.git)

**The Architecture:**

Built the foundation using Terraform modules to provision a complete AWS EKS cluster with properly segmented VPC, subnets across multiple availability zones, and all necessary IAM roles and security groups. This infrastructure-as-code approach enabled consistent, repeatable deployments.

Then integrated Ansible for configuration management and application deployment. Mastered Ansible's `kubernetes.core.k8s` module and its prerequisites (python3, pyYAML, Kubernetes Python client, jsonpatch). Automated kubeconfig generation and environment variable configuration to enable seam


## Monitoring with Prometheus and Grafana

Implemented a comprehensive monitoring solution for containerized applications on AWS EKS, providing full visibility into cluster health, application performance, and infrastructure metrics. Configured proactive alerting to catch issues before they impact users.

[View Project Repository →](https://gitlab.com/my-capstone-projects-devops/monitoring-with-prometheus-and-grafana)

**What I Built:**

Deployed Prometheus in Kubernetes to collect metrics from multiple layers—cluster health, pod resource usage, application performance, and infrastructure components. Built custom Grafana dashboards to visualize system health and performance trends, making it easy to spot issues at a glance.

Configured proactive alert rules for high resource usage, pod crashes, and service unavailability. Created custom dashboards for quick troubleshooting and issue identification. Tuned alerts to be actionable rather than noisy—catching problems before users noticed them.

**Technologies:** Prometheus • Grafana • Kubernetes (EKS) • AWS • PromQL • Linux

**Key Learnings:** Installed and configured Prometheus within Kubernetes clusters, wrote PromQL queries to extract meaningful metrics, designed intuitive Grafana dashboards for system visibility, configured alerting rules that balance sensitivity with actionability, and understood how proper observability transforms reactive firefighting into proactive problem detection.

**The Impact:** This monitoring stack provides the visibility needed to move from learning about issues through user complaints to detecting and fixing problems proactively. It drastically reduces mean time to detection (MTTD) and makes troubleshooting faster by showing exactly what's failing and when.


