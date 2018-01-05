# deployment-checklist
## Rails App
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
## SPAs 
- Setup GitHub Repo
  - Manage repo permissions 
- AWS Hosting
- Setup S3 Bucket
  - configure IAM 
- Route53 configuration
- Deployment Tool configuration ???
