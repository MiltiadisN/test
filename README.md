# AWS Cognito Angular   
# Description 
This project demonstrate how to integrate AWS services, including Lambda, Cognito, and API Gateway, into an Angular frontend.   
The application provides a robust authentication and authorization system using Amazon Cognito, allowing users to sign up, sign in, logout,     
reset their passwords, and receive verification codes. The UI is built with Bootstrap.    
This project was generated with Angular CLI version 16.0.5.

# Dependencies      
- Node.js and npm installed on your system
- AWS account to create a Cognito User Pool and manage Lambda functions and API Gateway.

# Technologies Used
- Angular: A powerful JavaScript framework used to develop the frontend of the application, providing a dynamic and reactive user interface.

- Amazon Cognito: A fully managed service by AWS that handles user registration, authentication, and user management.

- AWS Lambda: Serverless compute service by AWS, enabling the execution of custom code without managing the underlying infrastructure.

- API Gateway: A service by AWS that provides a secure and scalable API endpoint to access the AWS Lambda functions.

- Bootstrap: A popular CSS framework that enhances the application's UI and responsiveness.




# Features      
- User Authentication: The app offers secure user authentication powered by Amazon Cognito, ensuring that users' sensitive data is protected.
- User Registration: New users can sign up and create an account by providing essential details and verifying their email addresses.
- User Login: Registered users can sign in using their credentials and access the application's protected resources.
- Forgot Password: In case users forget their passwords, the application allows them to reset their passwords by receiving a verification code through email.
- Resend Verification Code: If users do not receive the verification code during the sign-up process, they can request a new code.
- AWS Lambda Integration: The application interacts with AWS Lambda functions via API Gateway, enabling seamless data processing and serverless computing.
- Responsive Design: The user interface is built with Bootstrap, ensuring that the application is accessible and user-friendly across various devices and screen sizes.





# Installation     
- Clone or download the project files.     
- Install the dependencies by running the following command in the project directory: **npm install** 
- Run the project: **ng serve**

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
