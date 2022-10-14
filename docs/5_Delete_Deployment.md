# (Optional for UDF users) Delete the Deployment

UDF users work in a controlled AWS environment which gets nuked soon as the UDF lab environment stops.

## Empty and delete the S3 bucket.
1. Navigate to `S3`.
2. Select the `cfeS3Bucket`. (It's the only bucket available)
3. Click Empty.
4. Delete the `Bucket`.

## Delete the demo application
1. Go to `EC2 > Instances`.
2. Select `f5-demo-app` and go to **Instance state > Terminate instance**
3. **Confirm** deletion.

## Delete BIG-IP deployment.
1. Navigate to **Cloudformation > Stacks**.
2. Select the `Parent template`.
3. Click **Delete** and **Confirm**.

Alternatively...
Use AWS CLI via the Jumphost Visual Studio.

**aws cloudformation delete-stack --region eu-central-1 --stack-name bigip-failover**

## Delete VPC
1. Go to `VPC`.
2. Select `bigip-vpc` and go to **Actions > Delete VPC**.
3. Delete the VPC.

This task is completed.


[PREVIOUS](../docs/4_App_Services_Deployment.md) [BacktoREADME](../README.md)