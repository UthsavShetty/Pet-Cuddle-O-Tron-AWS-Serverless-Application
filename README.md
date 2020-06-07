# Pet-Cuddle-O-Tron-AWS-Serverless-Application

#### Objective
In this demo, Implemented a serverless application using Step Functions, Lambda, SNS, SES, Api Gateway and S3 static web hosting. The application will be serverless and event driven and use no base long running compute while inactive. Resources will only be consumed when the application is dealing with user created events - the application being used.



#### Block Diagram
![image](https://user-images.githubusercontent.com/47194856/83961240-2be4dd00-a85f-11ea-8d4e-ba2c8507f151.png)




#### Webpage
![image](https://user-images.githubusercontent.com/47194856/83961278-78301d00-a85f-11ea-8428-56dc344d897d.png)





##### Flow
- If I press any of these blue buttons in event driven way, It will use javascript to make a call to the API Getaway, API Getaway will invoke Lambda functions which provides supporting services for this API.
- Lambda function will be provided with all this information that I've entered on this form and will use that to execute the state machine and the state machine will then wait based on how many seconds I specified in this boxand then it'll take a choice.
- It will either go with email only, SMS only or both, depending on which button I click at the bottom and then based on that, It'll interact with the Lambda to send the email and communicate with the SNS directly to send the text message.





