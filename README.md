# Create-Ecosystem-Big-Data-in-the-Cloud
DIO_Cloud_Data_Engineer
Dio Live Coding Code Repository with AWS EMR and Python This repository contains the data analysis configuration and execution files.

Instructions
Access S3: https://s3.console.aws.amazon.com/s3/
Create data lake structure : dio-live-datatake
Create folder structure:
date
output
temp
Access EMR: https://console.aws.amazon.com/elasticmapreduce/
The cluster will be created by MrJob and not the console
infrastructure as code
Create SSH Key
Access EC2 Console: https://console.aws.amazon.com/ec2/ -> Key Pairs -> Create Key Pair
Download .pem file
Get AWS Id and Secret Key to configure MrJob
Profile
My Security Credentials: https://console.aws.amazon.com/iam/home?region={region}#/security_credentials
Access Keys - Create new access key
Download - only chance to view
Linux environment
Create virtual python environment: virtualenv --python=python3.6 venv_diolive
Access with vs code
Install vscode on Ubuntu
code .
Create word analysis algorithm
dio-live-wordcount-test.py
map-reduce-count : count
Install boto3: pip install boto3
Install mrjob: pip install mrjob
Access S3
Upload file to bucket
Python virtual environment: source venv_teste/bin/activate
nano ~/.mrjob.conf
python3 dio-live-wordcount-test.py -r emr s3://{your_s3_bucket_name}/data/SherlockHolmes.txt --output-dir=s3://{your_s3_bucket_name}/output/logs1 --cloud-tmp-dir =s3://{your_s3_bucket_name}/temp/
