# EmailGenerationApp
This Email Generation App is a Java-based console application designed to generate unique email addresses and secure passwords for employees, typically for use by HR in organizations. The application is cloud-deployed on AWS, ensuring scalability, security, and monitoring via AWS services.

Project Overview
This application automatically generates and manages employee email addresses and passwords based on their names, ensuring no duplicates even with similar names. Hosted on an Amazon EC2 instance, it leverages AWS CloudWatch for monitoring and IAM for access management, making it a robust cloud-integrated solution suitable for organizational needs.

Features
Unique Email Generation:

Generates email addresses using the first initial of the first name and the full last name, appending a number if necessary to ensure uniqueness.
Random Password Generation:

Creates secure, random passwords for employees, which can be customized.
Password Strength Checker:

Ensures user-defined passwords meet basic security criteria.
Employee Management:

Allows for adding employees and displaying all registered employees with their details.
Architecture and AWS Integrations
1. Deployment on EC2
The application is deployed on an AWS EC2 instance, which provides a scalable and secure environment for cloud hosting. EC2 enables remote access to the application and offers cloud-based computing power, supporting the Java console application for generating emails and managing employees.

2. CloudWatch Monitoring
AWS CloudWatch is configured to monitor the EC2 instance, providing detailed insights into metrics like CPU usage and system logs. Alarms are set to notify on high CPU utilization, helping ensure performance optimization and troubleshooting. This integration enhances application reliability and gives visibility into runtime metrics.

3. IAM Security
AWS IAM (Identity and Access Management) is used to securely manage permissions and access to AWS resources. IAM roles are applied to the EC2 instance to restrict and control access, ensuring only specific services like CloudWatch have the necessary permissions. This setup ensures that the application’s cloud resources are accessed securely and efficiently.

Usage Instructions
Prerequisites
Java Development Kit (JDK) 8 or higher
AWS CLI (for managing AWS resources, optional for monitoring and permissions)

