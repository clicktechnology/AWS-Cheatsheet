
# AMAZON AWS

## Platforms and LAN
| Term | Expansion/Meaning | Example/Real life |
|-------|------------|-----------|
| Region | A geographical place | US-WEST-1 |
| Availability Zone | A datacentre in a Region | US-WEST-1A, US-WEST-1B, US-WEST-1C |
| Amazon EC2 | Elastic Compute Cloud | VMs |
| Amazon ECS | Elastic Container Service | Docker |
| Amazon EKS | Elastic Kubernetes Service | Kubernetes |
| Amazon Fargate | Run containers without managing servers or clusters |
| Amazon SQS | Simple Queue Service | Message Queue Service, RabbitMQ |
| Amazon SNS | Simple Notification Service | Push Notification Service |
| VPC | Virtual Private Cloud | VLAN |
| VPG | Virtual Private Gateway | VPN Host |
| IGW | Internet Gateway | Router / Firewall |
| AWS Direct Connect | Direct Fibre Connection | E1/E3 Fibre leased line |
| Security Group | Stateful instance access control group | iptables -m owner --gid-owner somegroup |
| Network ACLS | Stateless control list | ciscorouter(config)#access-list 101 deny icmp any any |

## Storage
| Term | Expansion/Meaning | Example/Real life |
|-------|------------|-----------|
| Amazon EBS | Elastic Block Store | Hard disks attached directly to the instance physical machine. |
| Amazon EBS Volume | Partition on an EBS |
| Amazon EFS | Elastic File System | Linux Logical Volume Manager (LVM) |
| Instance Storage | VM (EC2 instance) runs on temporary VDisk | vdisk |
| Amazon S3 | Object Storage | SSD storage for things that won't get edited, eg images, pdfs, fixed data tc. |
| Amazon S3IA | Infrequent Access | HDD Storage on old disks on old hardware. Available data, but slow. |
| Amazon S3 Glacier | Ooooold data | Tape robot |


## Databases
| Term | Expansion/Meaning | Example/Real life |
|-------|------------|-----------|
| Amazon RDS | Relational Database Service | Postgres, MySQL servers |
| Amazon Dynamo | NoSQL Database | Mongo, CouchDB |
| Amazon Redshift | Data warehouse | Search data you're already finished with. |
| Amazon DMS | Database Migration Services | Move your data to the cloud, switch engines too if needed / ake db copies for dev. |
| AWS Neptune | GraphQL Database | GraphQL |

## Other..
| Term | Expansion/Meaning | Example/Real life |
|-------|------------|-----------|
| Amazon Route53 | DNS with extras | bind9 |
| Amazon Organisations | Manage multiple AWS accounts for billing / usage / policy etc. |
| Amazon Artifact | Inherit your compliance standards from Amazon infrastructure |
| AWS Shield | DDOS protection |
| Amazon Inspector | Auto audit your setups for mistakes |
| Amazon Guard Duty | Threat identification |
| AWS CloudTrail | Logs all API calls to your account userspace. |
| AWS AMI | Amazon Machine Image | Disk image of OS |
| AWS Lex | Bots |
| AWS SageMaker | Machine Learning |
| Amazon WAF | Well Architechted Framework |
| Amazon A2I | Amazon Augmented AI (Amazon A2I) provides built-in human review workflows for machine learning use cases.
| Amazon Quicksight | The most popular cloud-native, serverless BI service |


# AMAZON AWS - 5 Pillars of Well Architected Framework

## CROPSS

### COST

https://docs.aws.amazon.com/wellarchitected/latest/cost-optimization-pillar/design-principles.html

 - Implement cloud financial management
 - Adopt a consumption model
 - Measure overall efficiency
 - Stop spending money on undifferentiated heavy lifting
 - Analyze and attribute expenditure

### RELIABILITY

https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/design-principles.html

 - Automatically recover from failure
 - Test recovery procedures
 - Scale horizontally to increase aggregate workload availability
 - Stop guessing capacity
 - Manage change in automation

### OPERATIONAL EXCELLENCE

https://docs.aws.amazon.com/wellarchitected/latest/operational-excellence-pillar/design-principles.html

 - Perform operations as code
 - Make frequent, small, reversible changes
 - Refine operations procedures frequently
 - Anticipate failure
 - Learn from all operational failures

### PERFORMANCE

https://docs.aws.amazon.com/wellarchitected/latest/performance-efficiency-pillar/design-principles.html

 - Democratize advanced technologies
 - Go global in minutes
 - Use serverless architectures
 - Experiment more often
 - Consider mechanical sympathy

### SECURITY

https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/security.html

 - Foundations
 - Identity and access management
 - Detection
 - Infrastructure protection
 - Data protection
 - Incident response


## SUSTAINABILITY

   - Right.

# AMAZON AWS - SHARED RESPONSIBILITY MODEL

https://docs.aws.amazon.com/wellarchitected/latest/sustainability-pillar/images/sustainability-in-the-cloud.jpeg

                       Data Design and Usage
                    Software Application Design
                  Platform Deployments and Scaling
          Data Storage | Code efficiency | Utilisation and Scaling
    -------------------------------------------------------------------
               Servers | Cooling | Water | Waste
                            Data Centres | Building
                      Electricity Supply | Materials
    -------------------------------------------------------------------

> Written with [StackEdit](https://stackedit.io/).
