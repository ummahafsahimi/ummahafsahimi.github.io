# Umma Hafsa Himi
### DevOps Practitioner | Operational Engineer | Technical Project Manager

## Contact
- **Email:** ummahafsahimi@gmail.com
- **Phone:** +1 236-777-4457 
- **LinkedIn:** linkedin.com/in/umma-hafsa-himi/  
- **GitLab Projects:** https://gitlab.com/my-capstone-projects-devops
- 
## Resume
[Download Resume](20260119-DevOps-Resume-Himi.pdf)

Hi, I'm a DevOps Engineer who loves turning manual processes into automated solutions. I work with AWS, Kubernetes, Terraform, and Jenkins to build reliable infrastructure that scales. Browse my projects to see how I approach real-world DevOps challenges.

### Kubernetes CI/CD Capstone Project: AWS EKS & ECR Integration

**Project Overview:**  
Built a production-grade CI/CD pipeline using Jenkins that automates the entire deployment workflow from code commit to Kubernetes cluster deployment.

**Pipeline Workflow:**
1. Automatically increments application version
2. Builds Java Maven application artifact
3. Creates Docker image from the application
4. Pushes Docker image to AWS Elastic Container Registry (ECR)
5. Deploys the latest application to AWS EKS cluster
6. Commits version updates back to Git for version control

**Technologies Used:**
- Kubernetes (EKS)
- Jenkins (Pipeline-as-Code)
- AWS EKS & ECR
- Java & Maven
- Docker
- Git
- Linux

**Key Learning Outcomes:**
- Created and configured AWS Elastic Container Registry (ECR) and understood its integration with EKS
- Implemented secure authentication between Jenkins and ECR using AWS credentials
- Automated Kubernetes deployments to EKS clusters directly from Jenkins pipelines
- Applied GitOps principles by committing version changes back to source control

**Architecture Highlights:**
This project demonstrates a complete DevOps workflow where code changes trigger automated builds, containerization, registry management, and orchestrated deployments—all with proper version control and zero manual intervention.

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


