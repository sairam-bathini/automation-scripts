#!/bin/bash

#####################
#Author: Sairam Bathini
#Date: 30-09-2023
#
#Version: v1
#
#This script will report the AWS resource usage
#####################

#aws EC2
#aws S3
#aws Lambda
#aws IAM users

set -x

#list s3 buckets

aws s3 ls> resourceTracker

#list EC2 instances

aws ec2 describe-instances>>resourceTracker

#list aws lambda functions

aws lambda list-functions>>resourceTracker

#list IAM users

aws iam list-users>>resourceTracker
