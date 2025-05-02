# IAM User & Group Management

This project demonstrates how to create and manage IAM users, groups, and policies in AWS.

---

## 🔧 What I Did

- Created IAM users via the AWS Management Console
- Created and assigned users to groups with different permissions
- Applied managed policies for secure access control (e.g., Read-Only, Admin)
- Configured group permissions for different roles (admin, read-only)

---

## 💻 Example IAM Policy (Read-only Access)

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "s3:ListBucket",
      "Resource": "arn:aws:s3:::your-bucket-name"
    },
    {
      "Effect": "Allow",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}
