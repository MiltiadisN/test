# AWS Cognito Angular   
# Description 
This project demonstrate how to integrate AWS services, including Lambda, Cognito, and API Gateway, into an Angular frontend.      
The application provides a authentication and authorization system using Amazon Cognito, allowing users to sign up, sign in, logout,        
reset their passwords, and receive verification codes. The UI is built with Bootstrap.      

# Technologies Used
- Angular (version: 16.1.7)
- Bootstrap (version: 5.3.0)

# AWS Services Used
- AWS Amplify
- Amazon Cognito
- AWS Lambda
- API Gateway
  
# Prerequisites       
- [Node.js](https://nodejs.org/en) and npm installed on your system
- [AWS account](https://aws.amazon.com/) to create a Cognito User Pool and manage Lambda functions with API Gateway.

# Installation     
- Clone or download the project files.     
- Install the dependencies by running the following command in the project directory: **npm install** 
- Run the project: **ng serve**

# Configuration
1. Open the **'environment.ts'** file located in src/environments. Replace the following placeholders with your actual values:  
   ![image](https://github.com/MiltiadisN/test/assets/103901423/920f1a1d-8c16-4af3-abd8-25511b60669f)
2. In the **order.service.ts** file located in src/app/services replace the URL with your actual API Gateway URL from AWS.
   ![image](https://github.com/MiltiadisN/test/assets/103901423/70c680f3-4536-4cd1-b79c-4e6f1f2b8dcb)

# Features      
**1. User Registration:** New users can sign up and create an account by providing e-mail and password.
  ![image](https://github.com/MiltiadisN/test/assets/103901423/739b415e-9c2c-4d93-866a-b2ce8d2fa282)    
  After successful registration, a verification code is automatically sent to the user's email for account verification.    
  Insert the verification code after the registration process.        
  ![image](https://github.com/MiltiadisN/test/assets/103901423/7b013dbb-41d0-4a27-8d06-85cbef54c837)   

**2. User Login:** Registered users can sign in using their credentials and access the application.                  
  ![image](https://github.com/MiltiadisN/test/assets/103901423/87750e69-86b3-4b07-aba7-b967b2652a94)  
  After signing in successfully, the user gains access to view their orders retrieved from an AWS Lambda function.   
  ![image](https://github.com/MiltiadisN/test/assets/103901423/69fc5782-3b42-48ba-ba76-b22b5a224a40)
  The user can log out from the application.      
  ![image](https://github.com/MiltiadisN/test/assets/103901423/a4aa180f-9b0d-43ed-b50c-0b9f78ebf255)

**3. Forgot Password:** In case users forget their passwords, the application allows them to reset their passwords by receiving a verification code through email.      
  ![image](https://github.com/MiltiadisN/test/assets/103901423/a4e13eb7-bcb5-4337-8777-8d37b4d55020) 

**4. Resend Code:** If users do not receive the verification code during the sign-up process, they will have the option to request a new code when          
  they sign in with their email and password in the login section.
  ![image](https://github.com/MiltiadisN/test/assets/103901423/6f644325-5b97-4a30-94f6-9e8c8388243f)




