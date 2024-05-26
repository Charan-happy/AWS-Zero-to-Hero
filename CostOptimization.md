

## cost management: The ability to give visibility of costs to keep them under control and to enable cost optimization
## cost optimization: The ability to run systems to deliver business value at the lowest possible price point

### overview
- use consolidated billing to aggregate spend from multiple accounts into a single bill and take advantage of volume discounts
- use cost allocation tags to group resources and track spend in business terms that make sense to you, by project, cost center, application, or environment
- cost explorer provides visibility into your AWS spend and aws budgets allow you to monitor and raises alarms when spending crosses defined thresholds

  #### AWS tools for cost visibility
  - AWS cosst explorer
  - AWS Budgets
  - cost anomaly detection
  - Monthly AWS Bill AWS Billing console
  - custom inhouse or thirdparty solutions
 

### cloud intelligence dashboards
- A series of in-depth and customizable dashboards that provide the most comprehensive cost and usage details to help you optimize cost, track usage goals, and achieve operational excellence.

- Easy to use
- secure
- in-depth
- cost-efficient

## Tools for right sizing and finding unused resources
- AWS Trusted Advisor, CUDOS, compute optimizer, EC2 Rightsizing Recommendations(Cost Explorer)
- AWS cloudwatch (review metrics such as CPU Utilization %)
- TSO Logic (for pre-migration on-prem to AWS resource mapping)
- 3 rd party tools (including by not limited to):
    Stax, densify, cloudfix
  
### Tools for increasing elasticity/automation
- Autoscaling
- AWS Instance Scheduler
- 3 rd party paid tools (including but not limited to) : Granulate, gorillastack, skedddly, parkmycloudAPI

## Tools for Reserved instances & saving plans
- AWS cost Explorer (coverage, utilisation, and recommendations)
- AWS Cost and usage reports (hourly and resource-level granularity)
- AWS Budgets (utilization and coverage threshold warnings via email or SNS)
- 3 rd party tools (including but not limited to ) : Cloudhealth, zesty, apptio

## Tools for EC2 spt
- AWS Ec2 fleet
- AWS Spot fleet, pot instance advisor
- EC2 spot labs
- 3 rd party tools (including but not limited to): Bidelastic and spot etc


## Tagging Benefits
- operational support
- Cost and usage allocation
- Automation
- Control and compilance

## Tagging strategy
- Identify a set of tags using cross functional teams
- Define a tagging naming standard & dictionary
    > env = dev/test/stg/prod
- publish the tagging dictionary
    > Feedback + Announce + Refer
- Define "rules of the game"
    > Deployment Automation
- Enforce the rules
    > Re-active enforcement
- start small and iterate

  Monthly
  - TagCoverage %
  - Un-allocated spend/usage
  - Tag dictionary review

### Tagging -Tools
- Turning on cost allocation tags
- Tag editor to bulk filter, add, and edit tags
- Tag policies in AWS organizations to improve governance

|Tool Name | Description |
|---|---|
|Billing console| Review AWS charges and invoices, enable billing reports|
|AWS Cost explorer| Visually analyze AWS spend across multiple dimensions|
|AWS Cost anomaly Detection| Automated cost anamaly detection and root cause analysis|
|AWS Budgets|Improve planning and cost control with flexible budgeting and forecasting|
|CID/CUDOS|in depth, granular, and recommendation-driven dashboards|
|Cost allocation tags| Enable tag keys to be used as dimensions in billing reports and cost explorer|
|Cost and usage report| Review most granular (hourly, resource level) cost and usage data|
|Pricing calculator|calculate cost based upon estimated usage of AWS services|
|Trusted Advisor|Review cost optimization recommendations produced by TA|
|Compute optimizer|Get recommendations to optimize your EC2, EBS, Autoscaling & lambda resorues based on their utilization metrics data|
|Workspaces cost optimizer| Monitor amazon workspaces usage and optimize costs|
|Instance Scheduler|Automate stop/start scheduled of your EC2 or RDS instances|
|AWS Cost labs| AWS well-architected cost labs|
