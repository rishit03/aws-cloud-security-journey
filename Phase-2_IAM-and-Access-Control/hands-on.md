# Hands-On for Phase-2 IAM-and-Access-Control

## ✅ S3 Bucket Setup
- [x] Created bucket `my-private-reports`
- [x] Uploaded test file `report.txt`

## ✅ IAM Policy Creation
- [x] Created customer-managed policy `S3ReadOnly-ReportsBucket`
- [x] Policy allows `s3:GetObject` and `s3:ListBucket` only on `my-private-reports`
- [x] Explicitly scoped to specific bucket ARN

## ✅ Policy Attachment & Testing
- [x] Attached policy to IAM user `cloud-admin`
- [x] Verified:
  - ✅ Can read objects in `my-private-reports`
  - ❌ Cannot access other buckets (Access Denied)

## 🛡️ Summary
- IAM access successfully restricted using least-privilege principles
- Policies tested and working as expected
