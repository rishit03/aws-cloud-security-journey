# 🧪 Phase 4: Secure Storage – Hands-on Log

## ✅ Secure S3 Bucket Setup
- [x] Created bucket: `secure-data-store`
- [x] Blocked all public access
- [x] Enabled versioning
- [x] Enabled server-side encryption (SSE-S3)
- [x] Uploaded test file: `secrets.txt`

## ✅ Access Control
- [x] Attached bucket policy: Allow only my IAM user
- [x] Verified denied access to unauthorized roles/users

## ✅ Logging & Lifecycle
- [x] Enabled access logs (write to `s3-logs-rishit`)
- [x] Created lifecycle rule: Archive to Glacier after 30 days
