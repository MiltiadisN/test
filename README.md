# AWS Cognito Angular   
# Description 
This project demonstrate how to integrate AWS services, including Lambda, Cognito, and API Gateway, into an Angular frontend.   
The application provides a robust authentication and authorization system using Amazon Cognito, allowing users to sign up, sign in, logout,     
reset their passwords, and receive verification codes. The UI is built with Bootstrap.    

# Prerequisites       
- Node.js and npm installed on your system
- Angular CLI(16.1.7)
- [AWS account](https://aws.amazon.com/) to create a Cognito User Pool and manage Lambda functions with API Gateway.

# Technologies Used
- Angular

- Amazon Cognito

- AWS Lambda

- API Gateway

- Bootstrap

# Installation     
- Clone or download the project files.     
- Install the dependencies by running the following command in the project directory: **npm install** 
- Run the project: **ng serve**

# Features      
**1.** User Registration: New users can sign up and create an account by providing essential details and verifying their email addresses.
  ![image](https://github.com/MiltiadisN/test/assets/103901423/b7216e73-375d-4c96-a8d4-90019da0cb3b)   
  After successful registration, a verification code is automatically sent to the user's email for account verification.   
 Insert the verification code immediately after the registration process.     
  ![image](https://github.com/MiltiadisN/test/assets/103901423/7b013dbb-41d0-4a27-8d06-85cbef54c837)   

**2.** User Login: Registered users can sign in using their credentials and access the application's protected resources.        
  ![image](https://github.com/MiltiadisN/test/assets/103901423/3b8f18a7-8c61-4e1a-acb2-040d272c9b51)  


**3.** Forgot Password: In case users forget their passwords, the application allows them to reset their passwords by receiving a verification code through email.      
  ![image](https://github.com/MiltiadisN/test/assets/103901423/cfe0c03f-cef3-4236-b2bc-cfb60a43421e)  

**4.** If users do not receive the verification code during the sign-up process, they will have the option to request a new code when          
       they sign in with their email and password in the login section.
       ![image](https://github.com/MiltiadisN/test/assets/103901423/ba214773-bf4f-4c91-bad3-f5a438b405fd)








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
