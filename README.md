# Serverless Data Engineering Pipeline

![pipeline](https://user-images.githubusercontent.com/44381361/79702164-cb7aeb80-8270-11ea-816e-0f6b2665a403.png)

### Cloud watch timer is called every minute and reads data from DynamoDB. The Producer Lambda function takes messages and puts in the SQS. Once that is done then the Consumer Lambda function does AI/Machine Learning.


  * Created a producer Lambda function in this project it is "serverlessApr19"; setting the admin role
  * Created an SQS (Simple Queued Service) for the producer function
  * Created a table named"fang" in DynamoDB
  * Deploying the function and monitoring it, checking the messages on SQS.
  * Created a  CloudWatch timer for every 1 minute

![sqs](https://user-images.githubusercontent.com/44381361/79702165-d2a1f980-8270-11ea-9ff0-3c54747f01f4.png)
### The SQS shows the messages.

  * Once that is done create the consumer function 
  * Sourcing a virtual environment and downloading all the dependencies for the python script
  * Deploying the consumer function and checking the logs, SQS and monitoring on the Lambda page.


![lambda](https://user-images.githubusercontent.com/44381361/79702173-ddf52500-8270-11ea-8f00-0eba509aa143.png)
### Consumer Lambda function for this project was on sentiment analysis.

  * Finally when everything looks functioning well; checking on S# for the last step i.e writing the S3 bucket created before with the sentiment analysis names

![s3](https://user-images.githubusercontent.com/44381361/79702177-e51c3300-8270-11ea-873d-27a8a77c5ece.png)
### Finally the data written in an S3 bucket


