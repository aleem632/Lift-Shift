# Lift-Shift Application WorkLoad
![Local Architect](https://github.com/aleem632/Lift-Shift/blob/6d99f524ec7c0460bfade81d8ded96025d939dc1/Lift-Shift.png)

### About AWS Project
- Multi tier Application Stack
- Host & Run On AWS Cloud for Production
- Lift & Shift Strategy
# Services
### Locally Running on Local Machine
- web Nginx
- Tomcat 8 
- Memcache
- RabbitMQ
- MySql
# AWS Services 
- EC2 Instance-- VM for Tomcat, Rabbitmq, Memcache
- ELB[Load Balancer]-- Nginx LB Replacement
- AutoScaling--Automation for VM scaling
- S3/EFS Storage--Shared storage
- Route 53--Privat DNS Service
# Flow of Exection
- Login to AWS Account
- Create key Pairs
- Create Security group
- Launch Instance with User data[Bash Scipts]
- Update IP to name mapping in route 53
- Build Application From source code 
- Upload to s3 bucket
- Download artifact to tomcat Ec2 Instance
- Setu ELB with Https
- Map Elb Endpoint to website name in Godaddy DNs
![AWS](https://github.com/aleem632/Lift-Shift/blob/8dc3578d4bfabd65b31ea7d40600763b12e2230b/Diagram/Lift-shift-AWS.png)





