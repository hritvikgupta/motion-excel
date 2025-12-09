# Security Policy

## Supported Versions

We actively support security updates for the following versions:

| Version | Supported          |
| ------- | ------------------ |
| Latest  | :white_check_mark: |
| < Latest| :x:                |

## Reporting a Vulnerability

We take the security of Motion Excel seriously. If you believe you have found a security vulnerability, please report it to us as described below.

### Please do NOT:

- Open a public GitHub issue
- Discuss the vulnerability in public forums
- Share the vulnerability with others until it has been resolved

### How to Report

Please report security vulnerabilities by emailing: **[Your Security Email]**

Include the following information in your report:

1. **Description**: A clear description of the vulnerability
2. **Steps to Reproduce**: Detailed steps to reproduce the issue
3. **Impact**: Potential impact of the vulnerability
4. **Suggested Fix**: If you have a suggested fix, please include it
5. **Proof of Concept**: If possible, include a proof of concept or exploit code (in a secure manner)

### What to Expect

- **Acknowledgment**: You will receive an acknowledgment within 48 hours
- **Initial Assessment**: We will provide an initial assessment within 7 days
- **Updates**: We will keep you informed of our progress
- **Resolution**: We will work to resolve the issue as quickly as possible

### Disclosure Policy

- We will work with you to understand and resolve the issue quickly
- We will credit you for the discovery (if desired) after the vulnerability is resolved
- We will not take legal action against security researchers who act in good faith

### Security Best Practices

When using Motion Excel, please follow these security best practices:

1. **Keep Dependencies Updated**: Regularly update your dependencies to the latest secure versions
2. **Environment Variables**: Never commit API keys or sensitive information to version control
3. **API Keys**: Rotate API keys regularly and use the principle of least privilege
4. **Docker Service**: If running the Docker service, ensure it's properly secured and not exposed to the public internet
5. **HTTPS**: Always use HTTPS in production environments
6. **Input Validation**: Validate and sanitize all user inputs
7. **Authentication**: Implement proper authentication and authorization for production use

### Known Security Considerations

- **Code Execution**: The Docker service executes code in isolated containers. Ensure proper security measures are in place when deploying
- **API Keys**: Store API keys securely and never expose them in client-side code
- **CORS**: Configure CORS properly to prevent unauthorized access
- **Rate Limiting**: Implement rate limiting for API endpoints in production

### Security Updates

Security updates will be released as patches to the latest version. We recommend:

- Staying on the latest version
- Subscribing to security advisories
- Monitoring the repository for security-related updates

### Contact

For security-related questions or concerns, please contact:

- **Email**: [Your Security Email]
- **GitHub Security Advisories**: [Enable on your repository]

Thank you for helping keep Motion Excel secure!
