---
title: "Worklog Week 1"
date: 2026-04-20
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Week 1 Goals:

- Get familiar with the internship environment and members of the First Cloud Journey program.
- Understand the basic concepts of Cloud Computing and the AWS service ecosystem.
- Get familiar with AWS Management Console and AWS CLI.
- Practice deploying and managing basic resources on AWS (EC2, EBS).

### Tasks for This Week:

| Day | Task                                                                                                                                                                                                  | Start Date | End Date   | Resources                                 |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | ----------------------------------------- |
| Mon | - Get acquainted with FCJ members <br> - Read and note the rules and regulations of the internship unit                                                                                               | 20/04/2026 | 20/04/2026 |                                           |
| Tue | - Learn about AWS and its service types <br>&emsp; + Compute <br>&emsp; + Storage <br>&emsp; + Networking <br>&emsp; + Database <br>&emsp; + ...                                                      | 21/04/2026 | 21/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Wed | - Create AWS Free Tier account <br> - Learn about AWS Console & AWS CLI <br> - **Practice:** <br>&emsp; + Create AWS account <br>&emsp; + Install & configure AWS CLI <br>&emsp; + How to use AWS CLI | 22/04/2026 | 22/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Thu | - Learn basic EC2: <br>&emsp; + Instance types <br>&emsp; + AMI <br>&emsp; + EBS <br>&emsp; + ... <br> - Ways to remote SSH into EC2 <br> - Learn about Elastic IP                                    | 23/04/2026 | 23/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| Fri | - **Practice:** <br>&emsp; + Create EC2 instance <br>&emsp; + Connect via SSH <br>&emsp; + Attach EBS volume                                                                                          | 24/04/2026 | 24/04/2026 | <https://cloudjourney.awsstudygroup.com/> |

---

### Week 1 Results:

#### Knowledge

- Understood the concept of Cloud Computing and AWS's role.
- Grasped the main service categories:
  - Compute (EC2)
  - Storage (S3, EBS)
  - Networking (VPC, Security Group)
  - Database (RDS)
- Understood the relationships between services in a cloud system.

---

#### Practice

- Successfully created an AWS Free Tier account.
- Got familiar with AWS Management Console:
  - Searching and accessing services
  - Managing resources

- Installed and configured AWS CLI:
  - Access Key
  - Secret Key
  - Default Region

- Executed basic commands:

```bash
  aws configure list
  aws ec2 describe-instances
  aws ec2 describe-regions
```

- Deployed EC2:
  - Created 01 EC2 instance (t2.micro - Free Tier)
  - Created and used a key pair (.pem)
  - Successfully connected via SSH to the instance

- Worked with EBS:
  - Created an EBS volume (8GB)
  - Attached it to the EC2 instance
  - Verified and mounted the volume

- Able to use both in parallel:
  - AWS Console (GUI)
  - AWS CLI

---

#### Challenges and Solutions

- **Challenges:**
  - SSH error when connecting to EC2 (Permission denied).
  - Did not fully understand how Security Groups work.
  - Confused about the region when configuring AWS CLI.

- **Solutions:**

  Set the correct permissions for the key file:

```bash
  chmod 400 key.pem
```

- Read the documentation and practiced repeatedly to understand Security Groups.
- Reconfigured the CLI:

```bash
  aws configure
```

---

#### Evidence

- AWS Console (EC2 instance running)
- Successful SSH terminal session
- AWS CLI command output
- EBS volume attached

Example:

![EC2 Instance](../images/ec2-instance.png)
![SSH EC2](../images/ssh-ec2.png)

---

#### Lessons Learned

- Better understanding of the Cloud model (IaaS).
- Got used to managing resources remotely.
- Learned how to troubleshoot errors when working with a new system.
- Recognized the differences between a local and a cloud environment.

---

#### Plans for Next Week

- Learn about AWS Networking (VPC, Subnet).
- Work with S3.
- Deploy a simple application on EC2.
