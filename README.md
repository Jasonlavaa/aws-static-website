 # aws-static-website

This project is a **personal static website** hosted on **AWS**.  
It serves as both a **resume/portfolio** and a **learning project** to practice cloud deployment using core AWS services.

AWS Services used:
- Amazon S3 – static web hosting for HTML, CSS, and images
- Amazon CloudFront – CDN for global delivery, HTTPS Support, and SEO optimization
- AWS Certificate Manager (ACM) – SSL/TLS certificate for secure browsing
- Amazon Route 53 – custom domain DNS management

Deployment steps:
1. Create an S3 bucket
   -Enabled static website hosting
   -uploaded HTML,CSS, and images to S3 bucket
2. Set Permissions
   -Configured bucket policy to allow ClounFront access
3. Set up CloudFront Distrubution
   -Linked to S3 bucket as origin
   -Enabled HTTPS using ACM to get a SSL/TLS Certificate
4.Domain Configuration
  -Added Custom domain in Route 53
  -Pointed DNS Records to CloudFront distrubution

Security:
Enabled HTTPS by getting a SSL/TLS certificate
Restricted AWS S3 bucket access/policy

Future Improvements:
1.Add a contact form using AWS Lambda, API Gateway, and AWS SES
