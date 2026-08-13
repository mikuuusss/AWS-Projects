This project demonstrates a serverless event-driven application built on AWS that automatically processes text files uploaded to Amazon S3.
When a file is uploaded, an AWS Lambda function written in Python is triggered to calculate the total number of words in the file. 
The result is then published to an Amazon SNS topic, which sends an email notification containing the word count. 
The workflow showcases AWS serverless architecture, event-driven processing, and cloud automation. 

AWS services used:
  AWS Lambda 
  Amazon S3 
  Amazon SNS 
  IAM 
  Amazon CloudWatch 
  Python 
  Boto3 
  Architecture

Project architecture:
Upload Text File 
↓ 
Amazon S3 Bucket 
↓ 
ObjectCreated Event 
↓ 
AWS Lambda Function 
(Python + Boto3 Script) 
↓ 
Count Words in Text File 
↓ 
Amazon SNS Topic 
↓ 
Email Notification Sent 
