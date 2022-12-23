# Introduction

This repository contains scripts to create:
- One EC2 with Docker, Docker-Compose and a Sample application
- Security Groups
- Mounted Volume for MongoDb
- Elastic IP

The scripts will create resources in: us-east-1

# How to run it
- export AWS_PROFILE=user1 # The name of the profile you want to use
- ./create-stack.sh

# How to clean up
- ./delete-stack.sh

# Cloud Formation

## EC2 User Guide
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/AWS_EC2.html

## EC2 Instance User Guide
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance.html

- AvailabilityZone
- ImageId
- InstanceType
- UserData

# Tips

## List profiles
 aws configure list-profiles

## Select profile
export AWS_PROFILE=user1

## Use a Profile for a specific aws command
--profile profile-name

## Make a sh file executable
sudo chmod +x filename.bin

## List all volumes on a machine
lsblk