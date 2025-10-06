# AWS-Cloud-Computing-Bootcamp-S3-Lambda-Integration

# Week 10 Task Report

## Objective
The goal of Week 10 was to create an **S3 bucket** that triggers a **Lambda function** whenever a new file is uploaded. The Lambda function logs the file information to **CloudWatch** and sends an **email notification** using **Amazon SES**.

---

## Steps Completed

1. **Created an S3 Bucket**  
   - Set up a new bucket in AWS to store files.

2. **Configured S3 Event Trigger**  
   - Configured the bucket to invoke the Lambda function on `ObjectCreated:Put` events (file uploads).

3. **Created a Lambda Function**  
   - Developed the Lambda function in **Python**.  
   - Added environment variables for the **SES sender** and **recipient email addresses**.

4. **Attached IAM Policies**  
   - Added necessary permissions to allow Lambda to access:
     - **S3** (for bucket event triggers)  
     - **SES** (to send emails)  
     - **CloudWatch** (to log file information)

5. **Deployed Lambda Function**  
   - The Lambda function logs the **file name** and **bucket name** to CloudWatch and sends a notification email via SES.

6. **Testing and Verification**  
   - Uploaded a file to the S3 bucket to trigger the Lambda function.  
   - Verified execution by checking:
     - CloudWatch logs (for logged file info)  
     - Receipt of a confirmation email from SES

---

## Deliverables

1. Screenshot of the **S3 bucket** showing the event trigger connected to Lambda.  
2. Screenshot of the **Lambda function code and configuration**, including environment variables.  
3. Proof of execution: **CloudWatch logs** or **SES email confirmation**.

---

## Conclusion
The task was successfully completed. The Lambda function now responds to file uploads in the S3 bucket, logs the events to CloudWatch, and sends email notifications using Amazon SES.

---

**Author:** Zibonele Mabaso  
**Week:** 10  
**Project:** AWS Cloud Computing Bootcamp – S3 & Lambda Integration

**LinkedIn:** [www.linkedin.com/in/mpendulo-mabaso-50a1b8315](https://www.linkedin.com/in/mpendulo-mabaso-50a1b8315)  
**GitHub:** [https://github.com/zibonelemabaso-jpg](https://github.com/zibonelemabaso-jpg)
