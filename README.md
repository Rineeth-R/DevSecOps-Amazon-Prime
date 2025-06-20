**Automated Deployment of Amazon Prime Video Clone on AWS EKS via DevSecOps implementation**

![Screenshot 2025-06-20 105044](https://github.com/user-attachments/assets/2b0bce67-e47e-478c-8f48-9357a007a97e)

**Key Responsibilities & Technical Implementations**

**1.Cloud Infrastructure Provisioning & Containerization (AWS EKS & Docker)**

- Provisioned an AWS EC2 instance (Ubuntu) to serve as the Jenkins controller.
- Set up Docker on the EC2 instance for containerization tasks.
- Configured an AWS EKS cluster with two m5.large worker nodes for high availability and scalability.
- Deployed the application as a Docker container, built from the source code, and pushed to Docker Hub.
- Utilized Kubernetes for orchestrating the deployment of the containerized application within the EKS cluster.

**2.Integrated Security Implementation (DevSecOps - Shift-Left Approach)**
- Integrated SonarQube for static code analysis, identifying bugs, vulnerabilities, and code smells.
- Implemented SonarQube Quality Gate within the Jenkins pipeline to enforce code quality and security standards.
- Utilized OWASP Dependency-Check for software composition analysis, scanning project dependencies for known vulnerabilities.
- Integrated Trivy for comprehensive container image scanning to detect vulnerabilities within the Docker images.
- Incorporated Docker Scout for in-depth analysis of Docker images, providing insights into vulnerabilities and potential fixes.

**3. Automated CI/CD Pipeline Orchestration (Jenkins)**
- Installed and configured Jenkins on the AWS EC2 instance.
- Developed a declarative Jenkins Pipeline script (Jenkinsfile) to automate the end-to-end DevSecOps workflow, including:
   -> Code Checkout: Retrieving source code from GitHub.
   -> SonarQube Analysis: Performing static code analysis and enforcing quality gates.
   -> OWASP Dependency Check: Scanning for vulnerable dependencies.
   -> Trivy Scan: Performing security scans on files.
   -> Docker Build & Push: Building the Docker image and pushing it to Docker Hub.
   -> Docker Scout: Scanning the Docker image for vulnerabilities.
   -> Kubernetes Deployment: Deploying the application to the EKS cluster.
- Configured Jenkins with necessary tools like JDK 17, Node.js 16, and Docker.
- Established secure authentication to Docker Hub and SonarQube server using Jenkins credentials.

**4. Kubernetes Deployment & Scaling**
- Configured Kubernetes deployments and services within the EKS cluster to ensure high availability and accessibility of the Prime Video Clone application.
- Automated the deployment of the application to AWS EKS, utilizing Argo CD for GitOps-driven continuous delivery.

**5. Automated Notification & Alerts**
- Configured Jenkins Extended Email Notification to provide real-time updates on pipeline status (success, failure).
- Automated the attachment of security scan reports (Trivy) and build logs to email notifications for detailed post-build analysis.

**Key Achievements**
- Successfully designed and implemented a fully automated DevSecOps pipeline for the Amazon Prime Video Clone application on AWS EKS.
- Achieved robust "shift-left" security by integrating SonarQube, OWASP Dependency-Check, Trivy, and Docker Scout into early pipeline stages, 
  proactively identifying and mitigating vulnerabilities.
- Ensured scalable and resilient application deployment through the strategic use of AWS EKS and Argo CD.
- Streamlined the software delivery lifecycle by automating build, security analysis, and deployment processes, significantly reducing manual effort and improving delivery speed.
- Provided comprehensive visibility into code quality, security posture, and build status through integrated tooling and automated reporting.


**Technical Stack & Tools**
Cloud Platforms: AWS (EC2, EKS)
CI/CD: Jenkins, Git, GitHub
Containerization: Docker, DockerHub, Kubernetes
Continuous Delivery: Argo CD
Security Tools: SonarQube, OWASP Dependency-Check, Trivy, Docker Scout
Programming & Scripting: Shell Scripting, JavaScript (Node.js application)
Build Tools: NPM
Runtime Environment: JDK 17, Node.js 16

**JENKINS STAGES**:-

![Screenshot 2025-06-20 021751](https://github.com/user-attachments/assets/15af1557-0d7d-4efb-aa19-0f66e4afe51b)

**SONARQUBE PASSED:-**

![Screenshot 2025-06-20 021858](https://github.com/user-attachments/assets/c0e730a6-2f2d-4402-8932-ae909e53a783)

**ARGOCD:-**

![Screenshot 2025-06-20 021622](https://github.com/user-attachments/assets/4b1ab585-7012-4985-a61d-86b05cc9ac2c)

![Screenshot 2025-06-20 122857](https://github.com/user-attachments/assets/870d65c1-d609-4e97-a18c-9ee5f32114d5)

**PROMETHEUS:-**

![Screenshot 2025-06-20 104833](https://github.com/user-attachments/assets/cda9b148-ad61-4617-acde-46d2780a1506)

**GRAFANA:-**

![Screenshot 2025-06-20 022758](https://github.com/user-attachments/assets/2e2e1fc5-a32b-4454-a8d4-aa8c50ce9628)



