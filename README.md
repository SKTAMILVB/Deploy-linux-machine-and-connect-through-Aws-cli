**Deploy Linux Instance and Access it Using AWS CLI**

✅ 1. Create One Linux Machine in AWS (EC2)

Prerequisites:
1.AWS account
2.IAM user with necessary EC2 permissions
3.Key pair for SSH login (we’ll generate one if not already available)

🟢 Step 1: Log in to AWS Console
Go to https://console.aws.amazon.com
Choose region (like us-east-1, ap-south-1, etc.)

🟢 Step 2: Launch EC2 Instance
Go to EC2 > Instances > Click Launch Instance

**Fill the details:**
1.Name: MyLinuxServer
2.AMI: Choose Amazon Linux 2023 (or Ubuntu if you prefer)
3.Instance type: t2.micro (free tier eligible)
4.Key pair: Create new or select existing key (e.g., my-key.pem).
5.Network Settings:
6.Allow SSH (port 22) from My IP
7.Click Launch Instance
8.After launch, note down the Public IP / DNS

✅ 2. Access the Server using AWS CLI
**Prerequisites:**
1.AWS CLI installed (Install AWS CLI)
2.IAM credentials configured using aws configure
3..pem key file for SSH
![image](https://github.com/user-attachments/assets/f63a0c8b-07a9-4641-84cc-d9997ad3699c)
1.AWS Access Key ID
2.AWS Secret Access Key
3.Region (e.g., ap-south-1)
4.Output format (e.g., json)
![image](https://github.com/user-attachments/assets/34bb8fdc-8d86-40ff-bd99-ea6435c8139d)
1.For Ubuntu: use ubuntu@<public-ip>
2.For Amazon Linux: use ec2-user@<public-ip>
![image](https://github.com/user-attachments/assets/ca0a0421-80af-4cb3-894d-1d507d1ada0d)

