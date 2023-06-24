# f5-aws-mp-gateway
This project provides a working configuration of NGINX configured to act as an authenticating gateway for integrating SaaS products listed on AWS Marketplace. This allows you to proxy a private AWS Marketplace SaaS APIs without requiring users to authenticate to it via AWS signature.

Within the proxy layer of f5-aws-mp-gateway, additional functionality can be configured such as:
- Providing an AWS signature based authentication gateway using an alternative authentication system to AWS Lambda functions
- For internal/micro services that can't authenticate against the AWS Marketplace SaaS products (e.g. don't have libraries available) the gateway can provide a means to accessing Marketplace SaaS products without authentication
- Protecting Marketplace SaaS products from arbitrary public access
- For internal/micro services that can't authenticate against the AWS Marketplace SaaS products
- Rate limiting AWS Marketplace SaaS products
- Authenticating users to authorize AWS Marketplace SaaS products with a OIDC
- Protecting AWS Marketplace SaaS products with a WAF


## References
- [AWS Marketplace Serverless SaaS Integration on AWS](https://aws.amazon.com/solutions/implementations/aws-marketplace-saas/)
- [GitHub: AWS Marketplace - Serverless integration for SaaS products (Example)](https://github.com/aws-samples/aws-marketplace-serverless-saas-integration)
