# Use-Case Questionnaire

This questionnaire is aimed to help you/us find the most suitable example or self-baked use-case.
Despite wanting only to trial it, we suggest that you deploy, and test it, in the most-similar situation to what
you have on your production environment.

We are aware that current examples don't suit all situations, and we will keep improving them to be as configurable as possible.
Contact us with these questions answered to help us.

> Sysdig Secure for Cloud is served in Terraform [AWS](https://github.com/sysdiglabs/terraform-aws-secure-for-cloud), [GCP](https://github.com/sysdiglabs/terraform-google-secure-for-cloud) and [Azure](https://github.com/sysdiglabs/terraform-azurerm-secure-for-cloud)
modules, and we also offer [AWS Cloudformation templates](https://github.com/sysdiglabs/aws-templates-secure-for-cloud)


- does your company work under an organization (AWS/GCP) or tenant (Azure)?
- if so, how many member accounts (aws) /projects (gcp) /subscriptions (azure) does it have?
- in what Sysdig features are you interested in?
    - [ ] [Runtime Threat Detection](https://docs.sysdig.com/en/docs/sysdig-secure/insights/)*
    - [ ] [Compliance](https://docs.sysdig.com/en/docs/sysdig-secure/posture/compliance/compliance-unified-/)* (cis benchmarks and others)
    - [ ] [Identity and Access Management](https://docs.sysdig.com/en/docs/sysdig-secure/posture/permissions-and-entitlements/)*
    - [ ] Registry/repository [Image scanning](https://docs.sysdig.com/en/docs/sysdig-secure/scanning/)
    - [ ] Runtime workload image scanning (ecs on Aws, cloudrun on GCP, or container instances on Azure)


for AWS using customers
  - [ ] do you have an existing cloudtrail?
    - if yes, is it an organizational cloudtrail?
      - does the cloudtrail report to an SNS?
    - if it's not organizational, does each trail report to the same s3 bucket?
  - sysdig secure for cloud is presented in different workload flavor; ECS, K8S or Apprunner, would you have any preference?
    - in case of ECS or K8S, do you have an existing cluster you would like to re-use?