# Cloud IAM: Permissions and Access Management

## Introduction

Google Cloud Identity and Access Management (IAM) is a service that enables administrators to control who can access specific Google Cloud resources and what actions they can perform. IAM provides centralized access control through roles and permissions, helping organizations secure their cloud environments. In this lab, different user roles were assigned, modified, and revoked to demonstrate how IAM controls access to Google Cloud resources.

## Objectives

* Understand the fundamentals of Google Cloud IAM.
* Explore project-level IAM roles and permissions.
* Grant access to users through IAM policies.
* Revoke user access from a Google Cloud project.
* Assign resource-specific permissions.
* Verify how IAM roles affect access to Cloud Storage resources.

## Key Steps Performed

### 1. Exploring IAM Roles

* Signed in using two separate user accounts with different permission levels.
* Examined project-level IAM roles including Owner and Viewer.
* Reviewed the permissions associated with each role.

### 2. Creating a Cloud Storage Bucket

* Created a new Cloud Storage bucket with a unique name.
* Configured the bucket using default settings.
* Uploaded a sample file to the bucket for access testing.

### 3. Verifying Viewer Access

* Confirmed that the second user with the Viewer role could view project resources.
* Verified visibility of the Cloud Storage bucket and uploaded file.

### 4. Revoking Project Access

* Removed the Viewer role assigned to the second user.
* Updated IAM policies to revoke project-level permissions.
* Verified that the second user could no longer access project resources.

### 5. Granting Resource-Specific Permissions

* Added the second user back with the Storage Object Viewer role.
* Assigned permissions specifically for Cloud Storage objects.
* Applied the updated IAM policy.

### 6. Testing Access Permissions

* Used Cloud Shell commands to verify access to bucket contents.
* Confirmed that the second user could view storage objects despite lacking project-level access.
* Validated the effectiveness of fine-grained IAM permissions.

## Results

The lab successfully demonstrated how Google Cloud IAM manages access through roles and permissions. Project-level access was granted and revoked using IAM policies, and resource-specific permissions were assigned through predefined roles. The results showed how IAM enables secure access control by allowing administrators to grant only the permissions required for specific tasks.

## Conclusion

This lab provided hands-on experience with Google Cloud IAM and role-based access control. By managing user permissions at both project and resource levels, the lab illustrated the principles of least privilege and secure cloud administration. The exercise highlighted the importance of IAM in protecting cloud resources while ensuring users have the appropriate level of access to perform their responsibilities.
