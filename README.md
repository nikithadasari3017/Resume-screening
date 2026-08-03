# Resume Screening Automation Using AWS

## 📖 Overview

Resume Screening Automation is a serverless cloud application developed using **Amazon Web Services (AWS)** and **Python** to simplify the recruitment process. The system automatically processes uploaded PDF resumes, extracts candidate information, stores the extracted data in a database, and sends email notifications to recruiters.

This project demonstrates the implementation of an event-driven, serverless architecture using AWS services, reducing manual effort and improving recruitment efficiency.

---

## ✨ Features

* Upload resumes in **PDF** format.
* Automatically trigger AWS Lambda when a resume is uploaded.
* Extract candidate information such as:

  * Name
  * Email Address
  * Skills
* Store extracted details in **Amazon DynamoDB**.
* Send automated email notifications using **Amazon SES**.
* Secure and scalable serverless architecture.
* Fast and efficient resume processing.

---

## 🏗️ Architecture

```text
Resume Upload
      │
      ▼
 Amazon S3 Bucket
      │
      ▼
 S3 Event Trigger
      │
      ▼
 AWS Lambda Function
      │
      ├──────────────► Amazon DynamoDB
      │                  (Stores Candidate Details)
      │
      └──────────────► Amazon SES
                         (Sends Email Notification)
```

---

## 🛠️ Technologies Used

### Cloud Services

* Amazon S3
* AWS Lambda
* Amazon DynamoDB
* Amazon SES
* AWS IAM

### Programming Language

* Python 3

### Libraries

* boto3
* PyPDF2
* json
* re

---

## ⚙️ How It Works

1. Upload a PDF resume to an Amazon S3 bucket.
2. The upload event triggers an AWS Lambda function.
3. Lambda extracts text from the resume using Python.
4. Candidate details such as name, email, and skills are identified.
5. The extracted information is stored in Amazon DynamoDB.
6. Amazon SES sends an email notification to the recruiter.
7. Recruiters receive structured candidate information without manually reviewing resumes.

---

## 📂 Project Structure

```text
Resume-Screening-AWS/
│── lambda_function.py
│── requirements.txt
│── README.md
│── architecture.png
└── sample_resume.pdf
```

---

## 🚀 Getting Started

### Prerequisites

* AWS Account
* Python 3.x
* AWS CLI (optional)
* Configured IAM Roles and Permissions

### AWS Services Required

* Amazon S3
* AWS Lambda
* Amazon DynamoDB
* Amazon SES
* IAM

---

## 💡 Skills Demonstrated

* Cloud Computing
* AWS Serverless Architecture
* Python Programming
* Event-Driven Applications
* Amazon S3
* AWS Lambda
* Amazon DynamoDB
* Amazon SES
* IAM Configuration
* PDF Processing
* Automation

---

## 🔮 Future Enhancements

* AI-powered resume ranking
* Skill matching with job descriptions
* OCR support for scanned resumes
* Resume summarization using Generative AI
* Recruiter dashboard with analytics
* Support for DOCX and other document formats

---

## 📸 Screenshots

Include screenshots of:

* Amazon S3 Bucket
* AWS Lambda Function
* DynamoDB Table
* Amazon SES Configuration
* Successful Email Notification
* Application Workflow

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome. Feel free to fork the repository, create a new branch, and submit a pull request.

---

## 📄 License

This project is intended for educational and learning purposes.

---

## 👩‍💻 Author

**Nikitha Dasari**

Final Year B.Tech Student | Cloud Computing Enthusiast

* GitHub: *Add your GitHub profile link*
* LinkedIn: *Add your LinkedIn profile link*

---

⭐ If you found this project useful, consider starring the repository!
