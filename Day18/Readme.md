AWS Cloudwatch Events and EventBridge

Amazon Event Bridge Dashboard walkthrough :

<details><summary>Developer Resources</summary>Learn<br>sandbox<br>quickstarts</details>
<details><summary>Buses</summary>Event buses <br> rules <br> Global endpoints <br> Archives <br> replays</details>
<details><summary>pipes</summary>pipes</details>
<details><summary>scheduler</summary>schedules <br> schedule groups</details>
<details><summary>Integration</summary>partner event sources <br> API Destinations</details>
<details><summary>schema registry</summary>schemas</details>

AWS Cloud Cost Optimization - Identifying Stale Resources
Identifying Stale EBS Snapshots
In this example, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instance and deletes them to save on storage costs.

Description:
The Lambda function fetches all EBS snapshots owned by the same account ('self') and also retrieves a list of active EC2 instances (running and stopped). For each snapshot, it checks if the associated volume (if exists) is not associated with any active instance. If it finds a stale snapshot, it deletes it, effectively optimizing storage costs.

[Documentation](https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-get-started.html)
