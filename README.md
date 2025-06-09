# EX - 4 IAM IDENTITY ACCESS MANAGEMENT IN CLOUD

## 🧪 AIM
To set up a private cloud environment in AWS using Amazon VPC, allowing for controlled, isolated networking and secure resource management within the AWS infrastructure.

---

## 📝 PROCEDURE

### 🔷 Phase 1: Planning the VPC

- **Define your use case**  
  Understand the application needs, security requirements, and compliance factors.

- **Plan IP address ranges**  
  Select a **CIDR block** that avoids conflicts with existing networks.

- **Select Availability Zones (AZs)**  
  Choose AZs for redundancy, fault tolerance, and optimized performance.

- **Plan internet connectivity**  
  Decide whether the VPC will have public internet access and how it will be configured (e.g., NAT, IGW).

- **Define security policies**  
  Determine required **security groups**, **network ACLs**, and **access control mechanisms**.

---

### 🔷 Phase 2: Create Your VPC

1. **Log in to AWS Console**  
   Go to **Services > VPC > Your VPCs**.

2. **Create VPC**  
   - Click **Create VPC**.
   - Enter VPC name and **CIDR block** (e.g., `10.0.0.0/16`).
   - Choose AZs and enable DNS settings as needed.

3. **Create Subnets**  
   - Add multiple subnets across AZs for resource segmentation.

4. **Configure Route Tables**  
   - Create route tables and associate with subnets.
   - Define routing logic for internal and external communication.

5. **Create Security Groups**  
   - Define inbound and outbound rules to control access to EC2, RDS, etc.

---

### 🔷 Phase 3: Deploying Resources

- **Launch EC2 Instances**  
  Deploy virtual machines inside the created subnets.

- **Set Up RDS Instances**  
  Create database services within private or public subnets.

- **Configure Networking**  
  Connect resources to subnets, route tables, and security groups.

- **Add Other Services (Optional)**  
  Integrate **S3**, **Lambda**, and other AWS services as needed.

---

### 🔷 Phase 4: Managing and Monitoring

- **Use AWS CloudWatch**  
  Monitor performance, uptime, and network activity.

- **Configure Logging**  
  Enable **VPC flow logs** and use **AWS CloudTrail** for audit trails.

- **Review Security**  
  Update security groups and monitor IAM roles regularly.

- **Scale Infrastructure**  
  Adjust instances and networking resources based on demand.

---

## 📸 OUTPUT

### Snapshot 1: Create VPC image

![op1](https://github.com/user-attachments/assets/f1bbe800-eb49-4fc4-a8b4-0b2c45b87da4)


### Snapshot 2: Configuring Subnets
![op2](https://github.com/user-attachments/assets/5c4d49dd-503e-44b7-8c00-783c7d7c9b16)

### Snapshot 3: Configure Subnets
![op3](https://github.com/user-attachments/assets/2dd70a6f-21c0-4390-9569-546792f76a81)

### Snapshot 4: Setting Internet gateway
![op4](https://github.com/user-attachments/assets/9531c864-6e80-40aa-91df-104d2a5724cc)

### Snapshot 5: Creating Internet gateway
![op5](https://github.com/user-attachments/assets/88a01fd1-add8-4f6e-a018-32d0d34edfcc)

### Snapshot 6: Setting Internet gateway
![op6](https://github.com/user-attachments/assets/b857ff77-0d91-4558-8327-c53a2887dce8)

### Snapshot 7: Creating route table

![op7](https://github.com/user-attachments/assets/5d9b8973-6962-465b-94e0-4ad0bc7f5db6)


### Snapshot 8: Configuring route table
![op8](https://github.com/user-attachments/assets/b70e1607-37e5-481a-92f2-543177903903)

### Snapshot 9: Editing routes

![op9](https://github.com/user-attachments/assets/fc6a6898-19bc-443f-93d7-369c9521ab1c)


### Snapshot 10: Creating route table
![op10](https://github.com/user-attachments/assets/75e0f1e3-cf04-45b5-a554-ee807f00c668)

## ✅ RESULT

A private cloud environment was successfully created in AWS using Amazon VPC. The VPC setup included subnets, route tables, internet gateways, and security groups to ensure secure, isolated, and scalable infrastructure management.
