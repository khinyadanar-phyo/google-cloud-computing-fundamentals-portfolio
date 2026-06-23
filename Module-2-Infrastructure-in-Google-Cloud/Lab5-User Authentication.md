# User Authentication with Identity-Aware Proxy (IAP) on Cloud Run

## Introduction

Identity-Aware Proxy (IAP) is a Google Cloud security service that controls access to web applications by authenticating users and authorizing requests before they reach the application. It enables secure access management without requiring developers to build custom authentication systems. In this lab, a Python-based web application was deployed on Cloud Run and secured using IAP. The application was enhanced to retrieve authenticated user information and verify user identities through cryptographic validation.

## Objectives

* Deploy a web application to Cloud Run using Python.
* Protect application access using Identity-Aware Proxy (IAP).
* Authenticate and authorize users before granting access.
* Retrieve authenticated user identity information from IAP.
* Verify user identity using cryptographically signed assertions.
* Understand secure authentication mechanisms in cloud environments.

## Key Steps Performed

### 1. Application Deployment

* Downloaded the lab source code and application files.
* Reviewed the Python application and HTML templates.
* Deployed the web application to Cloud Run.
* Verified successful deployment through the generated service URL.

### 2. Configuring Identity-Aware Proxy

* Enabled the Identity-Aware Proxy API.
* Activated IAP protection for the Cloud Run service.
* Added authorized users through IAM policies.
* Tested access restrictions and verified authentication requirements.

### 3. Accessing User Identity Information

* Modified the application to retrieve user information from IAP headers.
* Captured authenticated user email addresses and unique user IDs.
* Displayed authenticated user information on the web application interface.
* Verified successful identity retrieval after user login.

### 4. Testing Authentication Behavior

* Disabled IAP temporarily to observe application behavior.
* Examined how identity headers could be spoofed when authentication protection is removed.
* Analyzed the security risks of relying solely on request headers.

### 5. Cryptographic Verification

* Configured JWT audience settings for the Cloud Run service.
* Implemented verification of signed identity assertions provided by IAP.
* Validated user information using Google's public signing keys.
* Ensured identity data could not be forged or modified by unauthorized users.

### 6. Final Security Validation

* Re-enabled IAP protection.
* Granted required permissions to the IAP service account.
* Verified authenticated user information through cryptographically validated tokens.
* Confirmed secure user authentication and identity verification.

## Results

A Cloud Run web application was successfully deployed and secured using Identity-Aware Proxy. Access control was enforced through authenticated user authorization, while user identity information was retrieved and displayed within the application. Cryptographic verification was implemented to validate identity assertions and prevent spoofing attempts. The lab demonstrated how IAP provides a secure and scalable authentication solution for cloud-hosted applications.

## Conclusion

This lab provided practical experience in implementing secure user authentication for cloud applications using Identity-Aware Proxy and Cloud Run. By combining access control, user identity retrieval, and cryptographic verification, the application achieved a robust authentication mechanism without requiring custom login functionality. The exercise highlighted the importance of identity validation and secure access management in modern cloud environments.
