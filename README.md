# Back up plan using s3 bucket

- add


# Python Boto3 with AWS and S3 Task
- https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html
<br> </br>

### To install python 3.9 + boto3 on instance
- Create an instance and SSH into it
<br> </br>
- Install python:
```
sudo add-apt-repository ppa:deadsnakes/ppa

sudo apt-get update

apt list | grep python3.9

sudo apt-get install python3.9

sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.9 1

sudo update-alternatives --config python3

alias python=python3

sudo apt install python3.9-distutils

curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py

python3.9 get-pip.py
```
- Install boto3: `pip install boto3`
<br> </br>
### Set up aws config

- install pip `sudo apt-get install python3-pip`
 - `python3 -m pip install awscli`
 - `sudo pip3 install awscli`
 <br> </br>
 - To access buckets, run `aws configure`
 <br> </br>
 - Follow the below steps to access s3 buckets
 		- AWS Access Key ID: (Keep private)
 		- AWS Secret Access Key: (Keep private)
 		- Default region name : eu-west-1
 		- Default output format: json
- To check list of buckets run `aws s3 ls`
<br> </br>
- --------------------------------------
- Once in aws config, open python in the instance by running `python`