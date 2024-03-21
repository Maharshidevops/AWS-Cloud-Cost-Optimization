AWS Cloud Cost Optimization 

We're creating a small program (Lambda function) that looks for EBS snapshots (backups) that are no longer needed. It works like this:

Get Snapshots: First, it gets a list of all the EBS snapshots owned by our account.
Get Active Instances: Then, it checks which EC2 instances are currently running or stopped.
Check Snapshots: For each snapshot, it looks to see if the associated storage (volume) is still linked to any active instance.
Delete Stale Snapshots: If it finds a snapshot that isn't being used by any active instance, it deletes it to free up space and save money on storage costs.
So, basically, this program helps us clean up old backups that we don't need anymore, making our storage more efficient and saving us some cash.

- How can we ccreate and a generate script in python?
- For that we have to go to AWS Boto3 documentation and search for ebs,ec2 and all of the nessesory function and
modify as per your needs. It requires basic python scripting knowledge too.
- You can also go to our friendly chat-gpt and asked for simplified code.
