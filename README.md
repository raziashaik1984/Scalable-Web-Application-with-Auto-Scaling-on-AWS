# Scalable-Web-Application-with-Auto-Scaling-on-AWS
This project showcases the deployment of an AWS infrastructure that automatically scales with demand, adhering to best practices for scalability and maintainability.
## Infrastructure Setup
**EC2 Instances:**
Deploy EC2 instances to run your web application.
Use security groups to allow HTTP/HTTPS traffic to instances.

**Elastic Load Balancer (ELB):**
Set up an ELB to distribute incoming traffic between your EC2 instances and the load balancer is publicly accessible.

**Auto Scaling Group (ASG):**
Creates an Auto Scaling group to manage EC2 instances dynamically.

Defines scaling policies based on metrics like CPU utilization or incoming traffic.

**Cloud Watch:**
Implements CloudWatch monitoring to track the performance of your EC2 instances and ELB.

Set up CloudWatch alarms to trigger Auto Scaling actions based on performance metrics.

## Prerequisites


Terraform installed on your local machine.

An AWS account with appropriate permissions.

## Usage
**1.Clone the Repository**
```
git clone https://github.com/raziashaik1984/Scalable-Web-Application-with-Auto-Scaling-on-AWS

cd Scalable-Web-Application-with-Auto-Scaling-on-AWS
```
**2. Initialize Terraform**
```
cd envs/dev
terraform init
```

**3. Review and Apply Changes**
```
terraform plan
terraform apply
```
**4. Cleanup**
To remove the infrastructure, run:
```
terraform destroy
```
**Contribution**

Feel free to contribute by opening issues or submitting pull requests to improve the project.

**Reference**

This project is referenced from 
Terraform Up & RunningWriting Infrastructure as Code-
**Yevgeniy Brikman**