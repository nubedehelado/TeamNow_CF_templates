# TeamNow_CF_templates
CloudFormation templates for potential Team Now lesson modules focusing on System Administration and Infrastructure as Code

Templates:

* VPCTemplate.json: Defines a Multi-AZ VPC with 2 public subnets and 2 private subnets.
* WebAppv1.json: Single EC2 instance running a simple PHP web app
* WebAppv2.json: Multi-AZ LAMP stack
* WebAppv3.json: Deploys CloudWatch Logs Agent in ASG LaunchConfiguration
* three_tier_webapp.json: Complete, functional version of broken_template.json, using an nginx reverse proxy webserver, an app server hosting Wordpress and a MySQL db
* broken_template.json: three_tier_webapp.json with the subsequent errors: 
  * hardcoded ami's for us-west-2
  * subnets are not specified for ASG's (only AZs)
  * reverse proxy sends traffic to an EC2 instance instead of the internal ELB

Future TODO:

* Serverless web app with Lambda and API Gateway with VPC support
* Break out RDS instance into its own modular template (maybe use as a way to highlight nested stacks vs application tiers utilizing lambda-backed custom resources)

