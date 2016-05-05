# TeamNow_CF_templates
CloudFormation templates for potential Team Now lesson modules focusing on System Administration and Infrastructure as Code

Templates:

VPCTemplate.json: Defines a Multi-AZ VPC with 2 public subnets and 2 private subnets.
WebAppv1.json: Single EC2 instance running a simple PHP web app
WebAppv2.json: Multi-AZ LAMP stack
WebAppv3.json: Deploys CloudWatch Logs Agent in ASG LaunchConfiguration

Future TODO:

* Serverless web app with Lambda and API Gateway with VPC support
* Break out RDS instance into its own modular template (maybe use as a way to highlight nested stacks vs application tiers utilizing lambda-backed custom resources)

