# Notes for Phase-2 IAM-and-Access-Control

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "s3:ListBucket",
      "Resource": "arn:aws:s3:::my-secure-bucket"
    }
  ]
}

| Field       | Meaning                                                               |
| ----------- | --------------------------------------------------------------------- |
| `Effect`    | `Allow` or `Deny`                                                     |
| `Action`    | What action is permitted (`s3:GetObject`, `ec2:StartInstances`, etc.) |
| `Resource`  | What AWS resource is affected (S3 bucket, EC2 instance, etc.)         |
| `Condition` | Optional – set time, IP, MFA, etc.                                    |

