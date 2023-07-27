# Cognito User Pool Integration with Angular Application  
# Description 
This project demonstrate the integration of AWS Cognito User Pool into an Angular application to handle user authentication and registration. 
This project was generated with Angular CLI version 16.0.5.

# Dependencies      
- Node.js and npm installed on your system
- AWS account to create a Cognito User Pool and manage Lambda functions and API Gateway.

# Installation     
- Clone or download the project files.     
- Install the dependencies by running the following command in the project directory: npm install

# Angular Services
- Cognito Service: This service provides methods for user authentication and registration. Import and use this service in your components to handle user-related operations.

# Angular Components
- Registration Page: Integrate this component into your application to allow users to register. The component communicates with the Cognito Service to send verification codes and validate emails.

- Login Page: Incorporate this component to enable user login. The component uses the Cognito Service to handle user authentication.

- Route Guard Service: Implement this service to restrict access to specific pages in your application. You can use CanActivate to control user access based on authentication status.

# AWS API Gateway and Lambda
- API Gateway and Lambda Setup: Follow the instructions to create an AWS API Gateway with a Lambda function to handle backend requests for your application. No authorization or authentication is demonstrated in this video; however, you can integrate Cognito User Pool authorization and authentication later.

- Authorized API Gateway: Learn how to create an API Gateway authorizer using AWS Cognito User Pool. The video demonstrates accessing a secured API Gateway with the help of a Cognito JWT token.

# Resend Validation Code Component
- Resend Validation Code: Implement this component to address the issue of unconfirmed user registrations. The component allows users to resend validation codes for email confirmation.

# Forgot Password Functionality
- Forgot Password Link: Add a "forgot password" link to your Angular application. This functionality sends a request to Cognito to reset the password. Users receive a code via email, and they can reset their password using the provided code.
