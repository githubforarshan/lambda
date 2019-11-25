#Demo

1 launch ec2 instance

2 Create an IAM policy for Lambda

for this purpose we use the Json policy document into policy editor
Refer to "Policy.JSON" file

3 Create an IAM role for Lambda and attach the above policy to this role

4 Open the Lambda console

6 Choose Author from scratch.

Under Basic information, add the following:

For Function name, enter a name that identifies it as the function used to stop your EC2 instances. For my instance I have given, "StopEC2Instances".
For Runtime, choose Python 3.7.

Under Permissions, expand Choose or create an execution role.

Under Execution role, choose Use an existing role.

Under Existing role, choose the IAM role that you created.

7 Choose Create function.

8 Then under Function code, Under the editor pane in the code editor (lambda_function). Paste the code that I have written in "Code" file that I have attached.

9 Now the next step is to test

10 In Lambda function choose Functions

11 Select the Name of the function that you have given

12 Select Action then Choose Test

13 In the Configure test event dialog, choose Create new test event.

14 Enter an Event name, and then choose Create.   

15 Click Test to execute function










