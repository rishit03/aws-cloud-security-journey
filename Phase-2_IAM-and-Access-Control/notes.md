# Notes for Phase-2 IAM-and-Access-Control

# 🔐 Phase 2: IAM & Access Control – Notes

## ✅ Key IAM Concepts
- **User**: Entity that can access AWS (human or service)
- **Group**: Collection of users with shared permissions
- **Role**: Assignable set of permissions (used with EC2, Lambda, etc.)
- **Policy**: JSON document that defines permissions

## ✅ IAM Policy Structure (JSON)
```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::example-bucket/*"
    }
  ]
}

| Field     | Description                                   |
| --------- | --------------------------------------------- |
| Version   | Policy language version (always 2012-10-17)   |
| Statement | Block that defines permissions                |
| Effect    | Allow or Deny                                 |
| Action    | API operations allowed (e.g., `s3:PutObject`) |
| Resource  | Target AWS resources (ARNs)                   |
| Condition | Optional; used for IP, MFA, time, etc.        |

