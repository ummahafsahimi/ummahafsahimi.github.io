# Umma Hafsa Himi
### DevOps Practitioner | Operational Engineer | Technical Project Manager
#### Resume:   [Download here](20260129-DevOps-Resume-Himi.pdf)  <br><br>


Hi, I'm a DevOps Engineer with 5 years of industrial experience in CI/CD, Git, Linux, Nexus, and Python, and I build reliable cloud‑native infrastructure using AWS, Kubernetes, Terraform, and Jenkins.  
I also bring a strong foundation in core DevOps principles—version control, automation, observability, infrastructure design, and system reliability—and that truly matter in real‑world engineering.  <br>  

You’re welcome to explore my work below to see how I tackle real‑world DevOps challenges through automation, efficiency, and devOps best practices


## Kubernetes CI/CD Capstone Project: AWS EKS & ECR Integration

Built a production-grade CI/CD pipeline using Jenkins that automates the entire deployment workflow—from code commit to Kubernetes cluster deployment. The pipeline automatically increments versions, builds Java Maven artifacts, creates Docker images, pushes to AWS ECR, deploys to EKS clusters, and commits version updates back to Git for complete version control.

[View Project Repository →](https://gitlab.com/my-capstone-projects-devops/kubernetes-demo-eks-ecr-integration-in-ci-cd-jenkins.git)

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

Integrated AWS ECR as the container registry and built a Jenkins CI/CD pipeline to automate the entire deployment workflow. Configured Kubernetes Horizontal Pod Autoscaler (min=1, regular=2, max=3) to scale based on load while optimizing costs dynamically.

**Technologies:** AWS EKS & ECR • Kubernetes • Docker • Helm • Jenkins • Java/Maven • MySQL • Fargate • Linux • Git

**Key Learnings:** Understood the differences between stateful and stateless application deployment strategies in Kubernetes, configured Persistent Volume Claims for database data persistence, leveraged AWS Fargate for serverless container execution, implemented Helm charts for repeatable deployments, configured Horizontal Pod Autoscaler for cost-effective scaling, and automated multi-component deployments through CI/CD pipelines.

**The Result:** A production-ready Kubernetes deployment that balances performance, reliability, and cost—automatically scaling resources based on demand while maintaining data persistence for stateful workloads. This demonstrates real-world cloud-native architecture patterns.


## Kubernetes Microservices Deployment with Helm

Deployed a production-grade microservices application (Google's Online Boutique demo) to a Linode LKE cluster, implementing DevOps best practices for security, scalability, and maintainability. Focused on understanding microservice architecture patterns and inter-service communication flows.

[View Project Repository →](https://gitlab.com/my-capstone-projects-devops/kubernetes-demo-helmchart-and-microservices.git)

**Architecture:**

Deployed a complete microservices application consisting of multiple interconnected services to Linode Kubernetes Engine (LKE). Created shared Helm charts to manage consistent deployments across all microservices, ensuring version control and repeatability. Implemented security best practices including network policies, RBAC, and secrets management for production readiness.

The project required deep understanding of how microservices communicate with each other—service discovery, load balancing, and data flow between frontend, backend, cart, checkout, payment, and Redis cache services.

**Technologies:** Linode LKE • Kubernetes • Helm • Redis • Linux • Microservices Architecture

**Key Learnings:** Created and configured shared Helm charts for consistent microservice deployments across multiple services, applied Kubernetes security best practices including network policies and RBAC for production environments, provisioned and managed Linode Kubernetes Engine clusters, and understood microservice communication patterns and service mesh concepts for distributed applications.

**The Result:** A production-ready microservices deployment demonstrating cloud-native architecture patterns, secure inter-service communication, and infrastructure-as-code practices using Helm. This project showcases how modern distributed applications are built and deployed at scale.



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

[View Project Repository →](https://gitlab.com/my-capstone-projects-devops/python-demo-website-monitoring-and-recovery-with-python.git)



## Ansible Capstone Project: Deploying Applications to Kubernetes (EKS)

Automated the complete workflow of provisioning AWS infrastructure and deploying applications to Kubernetes using a combination of Terraform and Ansible. Demonstrated how infrastructure-as-code and configuration management tools work together to create fully automated, repeatable deployments.

[View Project Repository →](https://gitlab.com/my-capstone-projects-devops/ansible-demo-deploy-application-to-kubernetes-eks.git)

**Architecture:**

Provisioned AWS EKS cluster and VPC infrastructure using Terraform (check the `eks` branch for IaC files). Then configured the EKS cluster and deployed an Nginx application using Ansible playbooks. Automated kubeconfig generation and environment variable configuration to enable seamless communication between Ansible and the remote Kubernetes cluster.

Built Ansible playbooks using the `kubernetes.core.k8s` module to create dedicated namespaces for proper isolation and deploy applications with Services for network exposure. The idempotent design ensures playbooks can run multiple times safely.

**Technologies:** Ansible • Terraform • AWS EKS • Kubernetes • Docker • Python • Git • Linux

**Key Learnings:** Mastered Ansible's `kubernetes.core.k8s` module and its prerequisites (python3, pyYAML, kubernetes, jsonpatch), automated namespace creation and application deployment in EKS clusters, generated and updated kubeconfig files programmatically for cluster authentication, configured environment variables like `KUBECONFIG` and `K8S_AUTH_KUBECONFIG` for tool integration, and understood how IaC (Terraform) and configuration management (Ansible) complement each other.

**The Result:** A fully automated deployment system where Terraform provisions the infrastructure and Ansible handles configuration and application deployment—all through code with zero manual intervention. This demonstrates production DevOps workflows combining multiple tools effectively.


## Monitoring with Prometheus and Grafana

Implemented a comprehensive monitoring solution for containerized applications on AWS EKS, providing full visibility into cluster health, application performance, and infrastructure metrics. Configured proactive alerting to catch issues before they impact users.

[View Project Repository →](https://gitlab.com/my-capstone-projects-devops/monitoring-with-prometheus-and-grafana)

**What I Built:**

Deployed Prometheus in Kubernetes to collect metrics from multiple layers—cluster health, pod resource usage, application performance, and infrastructure components. Built custom Grafana dashboards to visualize system health and performance trends, making it easy to spot issues at a glance.

Configured proactive alert rules for high resource usage, pod crashes, and service unavailability. Created custom dashboards for quick troubleshooting and issue identification. Tuned alerts to be actionable rather than noisy—catching problems before users noticed them.

**Technologies:** Prometheus • Grafana • Kubernetes (EKS) • AWS • PromQL • Linux

**Key Learnings:** Installed and configured Prometheus within Kubernetes clusters, wrote PromQL queries to extract meaningful metrics, designed intuitive Grafana dashboards for system visibility, configured alerting rules that balance sensitivity with actionability, and understood how proper observability transforms reactive firefighting into proactive problem detection.

**The Impact:** This monitoring stack provides the visibility needed to move from learning about issues through user complaints to detecting and fixing problems proactively. It drastically reduces mean time to detection (MTTD) and makes troubleshooting faster by showing exactly what's failing and when.


### Contact
- **Email:** ummahafsahimi@gmail.com
- **Phone:** +1 236-777-4457 
- **LinkedIn:** linkedin.com/in/umma-hafsa-himi/  
- **GitLab Projects:** https://gitlab.com/my-capstone-projects-devops
  
