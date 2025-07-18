# cloud-task-3
# CLOUD COMPUTING 
**COMPANY**: CODTECH IT SOLUTIONS
**NAME**: PRINCE KUMAR 
**INTERN ID**: CT08DG546
**DOMAIN**:: Cloud Computing
**DURATION**: 8 WEEKS
**MENTOR**: NEELA SANTOSH


# Task 3 - Multi-Cloud Architecture
## Steps Completed:
1. Designed a multi-cloud setup using AWS S3 + GCP Cloud Functions.
2. Created architecture diagram.
2
3. Tested file flow from AWS to GCP.
## Why Multi-Cloud?
- Avoid vendor lock-in.
- Better uptime.
- Flexibility to use best services.

I designed a simple multi-cloud architecture to show how services from two cloud providers can work together — in this case, AWS S3 and Google Cloud Functions. Multi-cloud means not depending entirely on one vendor, which helps companies improve reliability, avoid vendor lock-in, and pick the best services for each requirement.

I used AWS S3 to store files (for example, images or PDFs). When a file is uploaded, S3 generates a public or signed URL. This URL is then used by a GCP Cloud Function, which is a serverless function that runs code in response to HTTP requests. I set up a simple HTTP-triggered Cloud Function on GCP that accepts the S3 URL, fetches the file from S3, and processes it (for example, logs the file metadata).

I created a clear architecture diagram showing this flow:
AWS S3 Bucket → File → Public URL → GCP Cloud Function → Process → Output.
I made this using an online diagram tool and added it to my project repository.

To prove this works, I also documented how to test the Cloud Function using its HTTP trigger. This task helped me learn how to connect different cloud services using standard HTTP methods, which is a core skill for designing real-world hybrid or multi-cloud systems. In an interview, I can explain the use case, why companies choose multi-cloud, and how I implemented a working example.

