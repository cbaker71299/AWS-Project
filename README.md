## **Project Overview**

During this cybersecurity internship, I was tasked with collaborating on a comprehensive project to design a secure and scalable three-tier web application infrastructure hosted in AWS for Georgia State University (GSU). The goal was to ensure the application’s robustness while maintaining compliance with key security frameworks. This project involved configuring a virtual private cloud (VPC), setting up the AWS environment, and conducting a detailed security assessment using various compliance standards.

## **AWS Infrastructure Design & Configuration**

To kick off the project, we worked together to set up the necessary AWS environment. This included creating a VPC that supported the three-tier web application architecture, using Amazon EC2 instances running on Amazon Linux 2023 AMI. We ensured that the EC2 instances were placed in both public and private subnets and configured with essential security controls such as restricted inbound traffic only on ports 22 (SSH), 80 (HTTP), and 443 (HTTPS). We also made sure the web services were resilient and could continue functioning in the event of an instance failure or if an entire Availability Zone (AZ) went down. To ensure fault tolerance and load balancing, we implemented automatic failover and balanced traffic across the EC2 web servers.

A crucial part of this configuration process was ensuring compliance with security best practices, including enabling Multi-Factor Authentication (MFA) across the AWS accounts and securing the EC2 instances. We ensured that the web server (httpd) was automatically installed when EC2 instances were created and configured all necessary VPC components to ensure smooth operation of the application. Throughout the project, we documented every step and used screenshots to present our work in a PowerPoint presentation.

## **Security Risk Assessment & Compliance**

Once the AWS environment was set up, our focus shifted to assessing its security posture. We used the Prowler tool to run a series of compliance assessments, specifically based on NIST 800-171 revision 2, as well as other frameworks like NIST 800-53, ISO 27001, and SOC2. The goal was to identify vulnerabilities and gaps in the AWS setup, particularly in relation to the sensitive data and regulatory requirements for educational institutions.

We then analyzed each finding from the Prowler assessments to evaluate the associated risks, including their likelihood and potential impact. By applying the NIST 800-171 framework, we were able to classify the findings and map them to control families and specific controls, allowing us to prioritize mitigation actions. Additionally, we used the NIST risk calculation equation to assess the severity of each risk and determined appropriate mitigation strategies. This involved using various types of risk mitigation, including risk avoidance, transfer, acceptance, and reduction, depending on the severity and potential impact of each issue.

## **Documentation & Presentations**

Throughout the entire project, clear communication was essential. We held weekly meetings with our client (the GSU cybersecurity team) and internally with our team, using Microsoft Teams. We provided detailed documentation of our findings and mitigation plans using Smartsheet, which helped us stay organized and ensure everyone was on the same page. We also created two detailed diagrams using Diagrams.net to represent the architecture of the VPC and the layers of the three-tier architecture. These diagrams were crucial in explaining the technical setup to both technical and non-technical stakeholders.

Finally, we compiled all our findings and mitigation recommendations into a comprehensive PowerPoint presentation. This presentation was structured to summarize our configuration process, present the risk assessment findings, and outline the proposed remediation steps to enhance the security of the AWS environment.

## **Conclusion**

This project was an invaluable learning experience in both cloud security and risk management. It allowed me to gain hands-on experience with AWS, deepen my understanding of security frameworks like NIST, and improve my ability to present complex technical information to non-technical stakeholders. By combining our efforts in designing, configuring, securing, and assessing the cloud infrastructure, we were able to deliver a secure, scalable, and compliant solution for GSU, demonstrating both technical and collaborative capabilities.
