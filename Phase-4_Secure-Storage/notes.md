# 📦 Phase 4: Secure Storage – Notes

## ✅ Key S3 Security Concepts

### 🔐 Access Control
- **IAM Policies**: Fine-grained, user/role-specific access
- **Bucket Policies**: JSON ACLs for cross-account/public access
- **ACLs**: Legacy; avoid unless needed

### 🔑 Encryption
- **SSE-S3**: Server-side encryption with S3-managed keys
- **SSE-KMS**: Server-side encryption with AWS KMS (recommended)
- **Client-side**: You encrypt before upload (less common)

### 🧱 Bucket Hardening
- Block all public access (default)
- Enable **versioning + MFA delete**
- Enable **server access logging**
- Use lifecycle rules for auto-archival/deletion

### 🕵️‍♂️ Logging & Monitoring
- S3 access logs: Write to another bucket
- CloudTrail: Track API-level events for S3
