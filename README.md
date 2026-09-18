<div align="center">

[![typing animation](https://readme-typing-svg.demolab.com/?font=Fira+Code&size=22&duration=2800&pause=800&color=2BBC8A&center=true&vCenter=true&width=640&lines=Systems+Engineer+%E2%86%92+Cloud%2FDevOps;Breaking+things+on+purpose+to+learn+how+they+fail;Documenting+the+journey%2C+one+practical+at+a+time)](https://github.com/tejasshinkar)

**[Projects](#-what-im-building-right-now)** · **[Previously Learned](#-previously-learned)** · **[Sharing Knowledge](#-sharing-knowledge)** · **[Stack](#-stack-i-actually-use)** · **[Contact](#-lets-talk)**

</div>


## → what I'm building right now

**[Automated EBS Snapshot Manager](🔲-add-repo-link)**: a Python automation system for backing up EBS volumes without babysitting the process.

- Identifies eligible volumes purely by tags, so nothing gets snapshotted, or skipped, by accident
- Creates each snapshot and tags it automatically, then enforces a retention window by deleting anything past it
- Runs on a schedule instead of manually, and logs every action to CloudWatch so there's an actual record of what ran and when

**[AWS IAM Access Audit Tool](🔲-add-repo-link)**: a Python script that scans an AWS account for the access issues that quietly turn into security debt.

- Flags IAM users without MFA, unused access keys, inactive accounts, and permissions broader than the role actually needs
- Built to run with read-only permissions wherever possible, since an audit tool shouldn't need write access to the thing it's auditing
- Uses IAM, Lambda/EC2, CloudWatch, and S3, producing an actual reviewable report rather than just flagging problems in a terminal
- The point isn't just detection. It's practicing least-privilege analysis the way it'd actually be reviewed in a real account

## → previously learned

| | |
|---|---|
| **Database architecture** | RDS Multi-AZ vs Read Replica, Aurora failover behavior, DynamoDB key design (partition/sort keys, GSIs, LSIs), and cache-aside patterns with ElastiCache — the trade-offs between availability, read scaling, and performance across relational and NoSQL |
| **Infrastructure as Code** | Practiced CloudFormation across progressively complex stacks, from a single EC2 instance to a self-healing ALB + Auto Scaling Group architecture |
| **Secure automation design** | Least-privilege IAM, idempotent scripting, and how a restricted permission model can change error behavior entirely (a missing-object check returning `403` instead of `404`) — the habits that separate a working script from something you'd trust unattended |
| **Event-driven architecture** | Wired S3 → Lambda, SNS → SQS with a dead-letter queue, and CloudWatch alarms → SNS notifications, then deliberately broke each one to learn exactly how it fails |

## → sharing knowledge

| Series | |
|---|---|
| **Networking Fundamentals** *(6 parts)* | [Series →](https://dev.to/tejas_shinkar/series/43298) |
| **AWS Cloud** *(18 parts)* | [Series →](https://dev.to/tejas_shinkar/series/40964) |
| **AWS Cloud: Hands-On Labs** *(8 parts)* | [Series →](https://dev.to/tejas_shinkar/series/43157) |
| **AWS Cloud Projects** *(3 parts)* | [Series →](https://dev.to/tejas_shinkar/series/43428) |
| **Python for Cloud and DevOps** *(10 parts)* | [Series →](https://dev.to/tejas_shinkar/series/40776) |
| **Tech After Dark** *(8 parts)* | [Series →](https://dev.to/tejas_shinkar/series/43607) |

## → stack I actually use

**cloud / infra**

![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white) ![EC2](https://img.shields.io/badge/AWS_EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white) ![S3](https://img.shields.io/badge/AWS_S3-569A31?style=flat-square&logo=amazons3&logoColor=white) ![Lambda](https://img.shields.io/badge/AWS_Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white) ![CloudFormation](https://img.shields.io/badge/CloudFormation-FF4F8B?style=flat-square&logo=amazonaws&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**databases**

![RDS](https://img.shields.io/badge/Amazon_RDS-527FFF?style=flat-square&logo=amazonrds&logoColor=white) ![Aurora](https://img.shields.io/badge/Aurora-232F3E?style=flat-square&logo=amazonaws&logoColor=white) ![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white) ![ElastiCache](https://img.shields.io/badge/ElastiCache_(Valkey)-DC382D?style=flat-square&logo=redis&logoColor=white)

**languages / automation**

![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=ffdd54) ![Boto3](https://img.shields.io/badge/Boto3-FF9900?style=flat-square&logo=amazonaws&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**day-to-day tools**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2671E5?style=flat-square&logo=githubactions&logoColor=white) ![Claude](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white)

**development background**

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Microservices](https://img.shields.io/badge/Microservices-4B275F?style=flat-square) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

full-stack roots, now focused on cloud/DevOps

currently deepening: Terraform, CI/CD pipelines, and AI-assisted cloud automation

## → let's talk

**[LinkedIn](🔲-add-linkedin-url)** · **[dev.to](https://dev.to/tejas_shinkar)** · **[Email](🔲-add-email)**

If I broke it on purpose, there's a write-up explaining why.
