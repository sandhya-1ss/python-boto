# python-boto
# AWS S3 Bucket Lister and Object Counter using Python (Boto3)
- Lists all S3 buckets in your AWS account.
- Displays the total number of objects in a specified S3 bucket.
##  Requirements

- AWS Account
- An EC2 instance (Amazon Linux 2 preferred)
- IAM Role with AmazonS3ReadOnlyAccess attached to the EC2 instance
- Python 3 and pip installed
- Boto3 library installed

## setup Instructions

1. Launch an EC2 Instance
- AMI: Amazon Linux 2 (Free tier eligible)
- Instance type: `t2.micro`
- Attach a key pair to SSH
- Attach a role with **AmazonS3ReadOnlyAccess**
-  SSH into the EC2 Instance
2.chmod 400 your-key.pem
ssh -i "your-key.pem" ec2-user@your-ec2-public-ip
3. Install Python 3 and pip
sudo yum update -y
sudo yum install python3-pip -y
4. Install Boto3
pip3 install boto3
5.Run
python3 list_s3_buckets.py
