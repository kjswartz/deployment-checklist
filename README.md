# deployment-checklist
# Rails App
- Setup GitHub Repo
  - Manage repo permissions 
- Setup Heroku
- Setup pipeline to GitHub repo
- Add heroku add-ons:
  - Redis (key/value cache store)
  - Logentries (simple log management vor viewing and searching)
  - New Relic (server status monitoring)
- Add proc file to rails app
- Mailer Setup
  - Mailchimp
- Asset Hosting
  - AWS S3 Bucket setup
    - configure IAM 

# SPAs 
## Github Repo
- [Setup GitHub Repo](https://help.github.com/articles/create-a-repo/)
- Configure permissions by [Managing Team](https://help.github.com/articles/managing-team-access-to-an-organization-repository/) access to an organization repository

## App Setup
- Use Webpack to ugilify
- Setup build/deploy script in package.json file for simple deploys
- Deployment Tool configuration ???

## AWS Hosting
Individual sections:
  - [Setup S3 Bucket](https://docs.aws.amazon.com/AmazonS3/latest/user-guide/create-configure-bucket.html)
  - [S3 Bucket Permissions](https://docs.aws.amazon.com/AmazonS3/latest/user-guide/set-permissions.html)
  - [Route 53](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/setting-up-route-53.html)

All S3 static site buckets should be configured with an Identity Access management (IAM) User. Set it up tied to the project name so the client is able to access. 
  - [Create IAM User](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html)
  
### [Complete AWS Setup Tutorial](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/getting-started.html)
This Getting Started tutorial shows you how to perform the following tasks:
  - Register a domain name, such as example.com
  - Create an Amazon S3 bucket and configure it to host a website
  - Create a sample website and save the file in your S3 bucket
  - Configure Amazon Route 53 to route traffic to your new website
