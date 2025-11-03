# DUMELANG <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28px" height="28px"> I'm Kemiso, Nice to Meet You
<p align="center">
  <img src="https://github.com/user-attachments/assets/23ec984e-282e-4126-bd01-cb3d47f75d37" alt="Adobe Express - TA-2025-11-03-12-09-createblow-810770351531136 (1)">
</p>

# <h2 align="left">👨🏻‍💻 Get To Know Me <img src="https://media.giphy.com/media/mGcNjsfWAjY5AEZNw6/giphy.gif" width="50"></h2>

From circuit board to secure cloud: My technical path is clear - I love Learning😄.
* **Specialization💡** I am an Electronic Engineer with a rare speciality in Artificial Intelligence/Machine Learning, Analogue/Digital Electronic Designs, and Signal & Systems 
* **Core Value⏳** Revolutionizing the world of digital communication for faster, more secure, and smarter communication across all sectors, from consumer electronics to healthcare.
* **Qualification/Certificate🎓** **AWS Certified Cloud Practitioner** & **Bachelors of Engineering**

## 🛠️ Core Competencies

* **Programming & Automation:** C++, Python, Bash shell, VHDL, PLC.
* **Cloud Technologies (AWS Focus):** EC2, S3, IAM, VPC, Lambda, ECS, Amazon Lex, SageMaker, Recognition, CloudFront, CloudFormation.
* **Operating Systems & Database:** Linux, CISCO IOS, SQL, NoSQL, RDBMS.
* **Tools:** MATLAB, Packet tracer, Git, AWS Management Console, Simulink, SCADA.
* **Electronics & Control Systems:** Analogue/Digital electronic design, PID controllers, broadband & mobile networks, robotics, Digital Signal Processing (DSP), IoT.
* **AI & Machine Learning:** Applied OpenCV, CNN, Haar cascade classifiers, LBPH face recognizer.
* **Project Management:** Led teams, delegated tasks, ensured timely project delivery.
* **Communication:** Fluent in English; beginner in Russian.
*  **Badge:**
  
<div align="center">
  <img width="300" height="300" alt="Aws Cloud Practitioner Badge" src="https://github.com/user-attachments/assets/7d093894-a288-415e-a16b-ed039907ccde" />
</div>

---

# 💡 My AWS re/Start Journey: From Ambition to Architecture

Welcome to my cloud playground! This repository is more than just code; it's a testament to my **12-week intensive transformation** through the **AWS re/Start program**. Having dedicated myself to mastering the fundamentals of cloud computing, networking, and security, I have emerged as an **AWS Certified Cloud Practitioner** ready to innovate and solve real-world challenges.

My journey taught me how to move beyond theoretical knowledge and apply **hands-on problem-solving** using core AWS services. I thrive in collaborative environments and I am committed to **continuous learning** in the ever-evolving world of cloud technology.

---

## 🌟 Core Competencies & Key Achievements

The AWS re/Start program is a rigorous, performance-based curriculum. I successfully navigated challenges that honed the following critical skills:

### ☁️ AWS Cloud Proficiency

* **Compute:** Launched, configured, and managed **EC2 instances**, utilizing **Auto Scaling Groups** for high availability and serverless **Lambda** functions for event-driven tasks.
* **Networking:** Mastered **VPC architecture**, including subnetting, routing tables, NAT gateways, **Security Groups**, and NACLs to build secure, isolated environments.
* **Storage:** Implemented **S3** solutions for durable object storage, configured lifecycle policies, and managed various **EBS** volumes and snapshots.
* **Databases:** Provisioned and managed relational databases (**PostgreSQL**) using **Amazon RDS** and explored NoSQL solutions with **DynamoDB**, enhanced with caching via DAX and ElastiCache.
* **Security & Monitoring:** Configured **IAM** roles and policies, and utilized **CloudWatch** and **Trusted Advisor** for robust monitoring, logging, and best-practice recommendations.

### 💻 Technical Skills & Tools

* **Languages & Scripting:** Proficient in **Python** and **Bash scripting** for automation tasks.
* **IaC (Infrastructure as Code):** Experienced in writing, validating, and deploying infrastructure via AWS **CloudFormation** templates (YAML/JSON).
* **Operating Systems:** High proficiency in **Linux CLI** commands and systems administration basics.
* **Version Control:** **Git & GitHub** for collaborative development and source control.

---

# 📂 Featured Projects

## 💾 Project 1: EBS Volume Lifecycle Management

This project demonstrates practical competence in managing the full lifecycle of **Amazon EBS (Elastic Block Store)** volumes, which provides durable, persistent storage for EC2 instances in the AWS Cloud.
https://github.com/KemisoInstances/The-12-Week-Cloud-Launchpad/blob/8f9f8758045114dab3c314a8365615592e92b76a/Projects/p1.md

### ⚙️ Step-by-Step Implementation

1.  **Create EBS Volume:** Provision the new block storage device in the **EC2 Console**. Ensure you select the correct **Availability Zone (AZ)**.
2.  **Attach Volume to Instance:** Connect the newly created volume to a running **EC2 instance** using the **Actions -> Attach Volume** menu option.
3.  **Connect to EC2:** Access the virtual server via **SSH** or **Session Manager** to prepare the storage.
4.  **Configure & Mount File System:** On the Linux instance, use commands (like `mkfs` and `mount`) to **create a file system** and then **mount** the volume to a directory, making the storage usable.
5.  **Create Snapshot:** Implement data protection. In the EC2 Console, select the mounted volume and choose **Actions -> Create Snapshot** to create a point-in-time backup.
6.  **Restore New Volume:** Perform disaster recovery. Navigate to the **Snapshots** section and choose **Actions -> Create Volume from Snapshot** to fully restore the data into a new EBS volume.
---
## 🌐 Project 2: Custom VPC Architecture & Web Server Deployment

https://github.com/KemisoInstances/The-12-Week-Cloud-Launchpad/blob/0a502aa55325f10129e8c8666aec953245314b90/Projects/p2.md
## ⚙️ Step-by-Step Implementation Guide

### Task 1: Create the Virtual Private Cloud (VPC)

1.  Navigate to the **VPC Console** and select **Create VPC**.
2.  Define a **CIDR block** (e.g., `10.0.0.0/16`) to specify the private IP address range for the network.

### Task 2: Create Subnets and Internet Gateway (IGW)

1.  **Create Subnets:** Create at least two subnets (Public and Private) across **two different Availability Zones (AZs)** for high availability. Assign appropriate CIDR blocks (e.g., `10.0.1.0/24`).
2.  **Create Internet Gateway (IGW):** Create the IGW and **Attach it to your VPC** to enable public internet connectivity.

### Task 3: Configure Route Tables and Auto-Assign IPs

1.  **Create Public Route Table:** Create a new Route Table and associate it with your VPC.
2.  **Add Internet Route:** Under **Routes**, add a route for destination `0.0.0.0/0` (all internet traffic) and point the target to your **Internet Gateway**.
3.  **Associate Subnets:** Go to **Subnet Associations** and explicitly associate your **Public Subnets** with this route table.
4.  **Enable Auto-Assign IP:** Navigate back to **Subnets**, select your Public Subnet(s), and **Enable auto-assign public IP** so EC2 instances receive a public address upon launch.

### Task 4: Launch Web Server (EC2) and Configure Security

1.  **Create Security Group (SG):** Create a new SG associated with your VPC. Add **Inbound Rules** to allow **HTTP (Port 80)** traffic from anywhere (`0.0.0.0/0`) and **SSH (Port 22)** access.
2.  **Launch EC2 Instance:**
    * Select an appropriate AMI and choose **Launch Instances**.
    * Under Network settings, select your custom **VPC** and one of the **Public Subnets**.
    * Select the **Security Group** created in the previous step.
    * Use **User Data** to install and configure a web server (e.g., Apache) upon startup.
3.  **Validation:** Once the instance is running, copy its **Public IP address** and paste it into a web browser to **verify the web server is publicly accessible**.
---
# 🔐 Project 3: AWS Identity and Access Management (IAM) Essentials

https://github.com/KemisoInstances/The-12-Week-Cloud-Launchpad/blob/fb29eca91deb42e74ce4181049147983b88626c5/Projects/p3.md

## ⚙️ Step-by-Step Tutorial

The project established a secure access framework using **IAM** by covering policy enforcement, user structuring, assignment, and real-world validation.

1.  **Enforce Password Security:** A custom **IAM password policy** was created and applied to mandate strong authentication across the AWS account.
2.  **Establish Permission Structure:** Explored the hierarchy of IAM **users and user groups** (like 'S3 Support') to understand how to efficiently manage permissions at scale.
3.  **Assign and Inspect Policies:** Specific **IAM policies** (e.g., `AmazonS3ReadOnlyAccess`) were attached to user groups to define explicit **Allow/Deny** actions for services based on the required job roles.
4.  **Validate Access Boundaries (Testing):** Users were assigned to their groups and logged in using the **IAM sign-in URL** to test permissions:
    * **User 1:** Confirmed being **denied EC2** operations while **allowed S3** access.
    * **User 2:** Confirmed being **denied S3** and denied the ability to stop EC2 instances, adhering to the **Read Only** policy.
    * **User 3:** Confirmed having **full administrative control** (e.g., successfully stopping an EC2 instance).
This sequence reinforced the critical necessity of the least privilege principle and effective access control in cloud environments.
---
# 🏗️ Project 4: Next-Generation 3D E-Commerce Platform Architecture

## 🦧Project Description
This project is designed to serves millions of global users. It demonstrates a deep understanding of multi-AZ deployments, automatic failover, edge caching, serverless components, and security best practices to achieve high availability, scalability, performance, and cost optimization.
https://github.com/KemisoInstances/The-12-Week-Cloud-Launchpad/blob/c98276ee7fd9cd8b607d7733c40a1b877076bd7f/Projects/Final%20Aws%20Project.md

---
### 🪐The platform was built using a layered approach, tracking a user's request from the network edge to the backend databases and back.

1.  **Global Entry and Security:** User requests first resolve via **Route 53 (DNS)**, directing traffic to **CloudFront (CDN)**. CloudFront serves cached content and uses **AWS WAF** to filter malicious requests before they enter the VPC.
2.  **Access Control:** Requests proceed to **API Gateway**, where **Amazon Cognito** handles authentication and authorization. Only verified, tokenized requests are allowed access to the compute layer.
3.  **Compute and Logic Execution:** The **Application Load Balancer (ALB)** routes requests to the appropriate service:
    * **Persistent Tasks** (core store logic) run on **EC2 instances** managed by an **Auto Scaling Group (ASG)** for resilience and scaling.
    * **Event-Driven Tasks** (background processes) run instantly via **AWS Lambda**, ensuring cost-efficiency.
4.  **Data Retrieval:** The compute services connect with the data layer, which uses specialized stores:
    * **DynamoDB** (accelerated by **DAX**) handles high-speed product catalog reads.
    * **RDS PostgreSQL** manages complex, transactional data like orders and inventory.
    * **ElastiCache** provides in-memory session caching for high performance.
5.  **Foundational Security:** All backend services are isolated within an **Amazon VPC**. **IAM Roles** strictly govern inter-service communication permissions, and **Security Groups** act as instance-level firewalls.
6.  **Visibility:** **CloudWatch** centrally collects all logs and metrics, providing continuous, real-time monitoring of the entire platform's health and performance.
---
## 📚 Key Labs & Hands-On Experiences

I have completed numerous hands-on labs (**scoring 1/1 on all graded assignments**) that simulate real-world scenarios. These labs were crucial in building practical expertise across various domains:

* **AWS Infrastructure & Management (JAWS/CF):** Configuring an Amazon VPC, Creating Amazon EC2 Instances, Scale and Load Balance your Architecture / Using Auto Scaling, and Automating Deployments with AWS CloudFormation.

* **Linux & Scripting Fundamentals (LX/PF):** Developed strong command-line proficiency through labs like Linux Command Line and Bash Shell Scripts.
* **Networking & Security (NF/SF):** Applied best practices in Network-Hardening, Systems-Hardening, and Introduction to **Identity and Access Management (IAM).**
* **Databases (DF):** Deployed and managed relational databases in labs such as Build Your Database Server.
---

## 🤝 Let's Connect & Collaborate

I am a team player with a problem-solving mindset and I am actively seeking opportunities to contribute my skills to an innovative team. 

* **Email:<img src="https://media.giphy.com/media/WUlplcMpOCEmTGBtBW/giphy.gif" width="30"> 
</em></p>** mareledioswardk@gmail.com

