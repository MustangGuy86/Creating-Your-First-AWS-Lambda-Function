# Creating-Your-First-AWS-Lambda-Function
In this lab, you will learn how to create your first AWS Lambda function, a serverless compute service that allows you to run code without managing servers. We will create a simple Lambda function that logs a message, and you'll learn the basic concepts of Lambda along the way.
Prerequisites
Before you begin, make sure you have the following:

An AWS account: You can sign up for one at AWS Sign-Up.
Basic understanding of the AWS Management Console.
Concepts
AWS Lambda
AWS Lambda is a serverless compute service that lets you run code without provisioning or managing servers. You can execute your code in response to various AWS events, such as changes to data in an S3 bucket, an update in a DynamoDB table, or even manually trigger it.

Node.js
Node.js is a runtime environment for executing JavaScript code outside a web browser. In this lab, we'll use Node.js as the runtime for our Lambda function.

Steps
1. Sign In to AWS Console
Go to the AWS Management Console at https://aws.amazon.com/console/.
Sign in with your AWS account credentials.
2. Navigate to Lambda
In the AWS Management Console, find and click on the "Services" menu at the top.
Under "Compute," select "Lambda" to open the Lambda dashboard.
3. Create a Lambda Function
Click the "Create function" button.
Choose "Author from scratch."
Configure the following:
Function name: Enter a unique name (e.g., "my-first-lambda").
Runtime: Choose "Node.js 14.x" (or any other runtime you prefer).
Execution role: Choose "Use an existing role" if you have one, or create a new role with basic Lambda permissions.
4. Create Function
Click the "Create function" button to create your Lambda function.
5. Write Code
In the Lambda function configuration, scroll down to the "Function code" section.
You can write or paste your Node.js code here. For example, you can create a simple Lambda function that logs a message.

exports.handler = async (event) => {
    console.log("Hello from Lambda!");
    return "Hello from Lambda!";
};


6. Test Your Lambda Function
Scroll up to the top of the Lambda configuration.
Click the "Test" button.
Configure a test event (e.g., "TestEvent") and click "Create."
Click the "Test" button again to execute your Lambda function.


7. View Execution Results
After running the test, you can view the execution results and logs in the "Execution results" section.


8. Clean Up (optional)
If you want to delete the Lambda function, you can do so from the Lambda dashboard.
Conclusion


Congratulations! You've successfully created and tested your first AWS Lambda function. Lambda is a powerful service for running code in response to events, and you can integrate it with other AWS services to build serverless applications.
