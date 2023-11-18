# AWS-Machine-Learning-Operations-MLOps

## Machine Learning Operations(MLOps) Introduction
### What is MLOps? </br>
What makes an AI most powerful today? For making insightful information and for prediction. Machine Learning is the process of teaching machine math methods.


## MLOps Motivation</br>
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/4d3d4748-87fa-428f-929d-6d3aa789b2df)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/884e6e06-4468-4cea-b749-36133eee6b85)
### High-Level View
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/387f524b-6969-4801-994a-a0e88b070246)


## MLOps Components</br>
### Typical workflow of creating an ML model
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/5447879d-e770-4aec-8f0b-fcf2e0473cec)
Model Register is used to version the ML models. </br>
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/658208c5-7d79-42e0-8974-c3def6aed3cb)
### Components
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/117f4291-e616-42c1-8784-8ab6e1535c92)

### MLOps Challenges
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/d58f6688-d18c-43ca-932a-96c46cc92c7f)
### DevOps vs MLOps
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/000fadbd-ee22-4275-8086-9edac3b0f28f)


## Automated ML pipelines vs CI/CD ML pipelines</br>
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/c5729fc6-bb9f-4aa1-9768-8fff968b1cc7)
Every organization has level 0 to level 4, which is called the maturity level of the machine learning model. Level 4 is the complete automated pipeline, as shown in the figure above. </br>
Feature Store: Here, we don't store our data. We store our versions here (Vewrsion a schema) during the model training stage. </br>
And monitor complete infrastructure for entire pipeline stages. Also, have a feedback loop (automated quality gates) to decide whether the model is better for the use case. </br>

### MLOps Stages
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/59a0cd6a-d85c-4140-8605-37ff578d368f)

### Different Roles involved in MLOps (ML Engineering + Operations)</br>
1. Versioning 
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/918dfd0c-bf51-45b7-9dee-6bf81d5cb016)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/a0a7a1f6-e17a-4b10-94fc-f423a25fb07d)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/a5b80a35-eef5-4652-86e8-942c97fcdbb2)
2. Testing in MLOps
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/39455a65-b13c-4f99-a15a-f4728cbc02df)
Unit Testing: Testing individual parts of the code. </br>
For Data Quality Testing: Evidently AI Tool </br>
3. Automation (CI/CD): for building, testing, and deploying the software.
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/8a3e793d-5d61-466a-910a-b54ab5306afc)
Here, the artifacts can be JAR files. These can also be the model files line pickle files. </br>

## Machine Learning Life Cycle</br>
### Steps involved in the CI/CD implementation in the ML lifecycle and workflow
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/35058dd8-6e21-4400-810e-dc89b8a6db51)

## Different tools for MLOps</br>
1. AWS CodeCommit
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/00191752-9b3e-4eff-a6f3-3634b90d8e54)
2. AWS CodePipeline (CD Tool: Also integrated with CI Tool)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/a9bb7d59-0b92-4177-8acb-995681dfaa62)
3. AWS CodeBuild (CI Tool)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/1256cea0-e7e8-4690-adea-c81485e36698)
4. AWS SageMaker: Complete Machine Learning platform provided by AWS. However, data is provided by AWS S3, which is an object storage platform.
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/3c3c0f3e-9cf6-447b-91f6-f2eea2b1d561)
### Object and Bucker in Amazon S3
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/21a248f1-4d7d-43d6-a4b6-c9cd47af03d0)


## Use Case</br>
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/eb34157e-6ad7-47ab-bb9c-804a751155d4)


## Getting started with AWS for Machine Learning
## AWS Machine Learning & AI Platforms Introduction</br>
## Amazon S3 introduction</br>
### Bucket Creation
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/a089be21-6275-47cf-a31d-31ae555d861a)
Editing Bucket Policy
```
{
	"Version": "2012-10-17",
	"Statement": [
		{
			"Sid": "PublicRead",
			"Effect": "Allow",
			"Principal": "*",
			"Action": "s3:GetObject",
			"Resource": "arn:aws:s3:::mlops-now/*"
		}
	]
}
```
Enable Static website hosting for S3 </br>]
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/77dc124f-a55f-4512-902d-c8ec09bb4343)
Enabling the bucket to be Public. </br>

## Amazon S3 for Machine Learning 
### Creating CodePipeline (Initial Version)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/00bfd8ff-fbc3-4b0c-a3fc-3ab999270c22)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/e9137910-2385-49d4-88de-e5744a03b5a3)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/f88b5ae9-293f-4f0d-a80e-56f3525561a3)

### Pipeline Running in Console
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/63b9f1b4-a527-4440-bc28-1bd999e5fa62)

### Checking for S3 Buckets Created
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/49c24f1c-9084-4751-a842-2bbf5fd80a96)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/d66284d7-32cc-4750-a422-5d746dc2aba1)

### Check for the End Point
```
[http://mlops-now.s3-website-us-east-1.amazonaws.com](http://mlops-now.s3-website-us-east-1.amazonaws.com/prod)
```

### Final Application of DevOps Pipeline
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/0f21c1b4-a678-42e2-ab36-0b4d3c34178a)

Source: WHERE WE ARE FETCHING OUR CODE
BUILDING OUR ARTIFACT
AND DEPLOYING OUT WEBAPP

### Making changes in GitHub code to check pipeline process
#### Commit Changes
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/0909def0-3fca-4268-bbb4-d35ecda93a3a)
#### Pipeline will trigger from start build process
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/3331a5a7-859a-4f4b-95a1-f00dca34c183)

#### Updated WebApp Page
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/a49f6ad6-9dda-40fc-b018-a6969899ac6b)

### Making changes to Pipeline
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/e83fc634-7d5d-4f4b-9e88-5e444339742d)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/25f8d62e-ceba-45e4-ab7b-dbd9c12f8ccf)

Make changes in GitHub again. </br>
After a few seconds, the pipeline will start executing. </br>
It shows that dev-approval is in progress. </br>
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/44e85980-abf8-4987-a53a-b3dd2e983f5d)

Approving Review for Dev
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/8287b92d-43b0-4b1a-bb17-19ad5c70411a)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/aecd22e2-048c-4fde-805a-6cb3bd13c568)

### S3 Bucket 
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/b76d6d03-4642-4094-92b7-e09975a893a2)

### Dev-Deploy WebApp
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/aa953c0c-4c4d-44e6-b341-d707105be646)

However, the production server will be serving the old app. After we approve the prod to be deployed, we get the updated prod web app server with new features.
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/61a6ad6d-8962-4389-b91e-34e0749824d3)

### Prod-Deploy WebApp
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/595a72bb-fe7f-4d74-a644-7f7d3e3101cb)

### Checking GitHub Commits
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/f5b36b73-1578-4b55-b77b-09cebdf75b91)
![image](https://github.com/srsapireddy/AWS-Machine-Learning-Operations-MLOps/assets/32967087/7160ab32-ecc9-42db-83a6-0b778375b499)


## AWS SageMaker
Introduction to Amazon Sagemaker</br>
Using Amazon S3 along with Sagemaker [Hands-on]</br>
Amazon SageMaker Notebooks and SDK [Hands-on]</br>
Notebook instance type, IAM Role & VPC [Hands-on]</br>
Build, Train & deploy ML Model using TensorFlow [Hands-on]</br>
Endpoint & Endpoint configurations [Hands-on]</br>
Generate inference from deployed model [Hands-on]</br>

## AWS Machine Learning Operations (MLOps)
Introduction Sagemaker pipelines</br>
AWS CodeCommit [Hands-on]</br>
AWS CodePipeline [Hands-on]</br>
AWS CodeBuild [Hands-on]</br>
Containers for Amazon SageMaker</br>
AWS MLOps - ML Model Monitoring</br>
AWS MLOps - Amazon Sagemaker Feature Store</br>
AWS MLOps - Post-Deployment Challenges</br>

## AWS MLOps - Build, Train & deploy ML Model
SageMaker Studio & SageMaker domain [Hands-on]</br>
SageMaker Projects [Hands-on]</br>
Repositories [Hands-on]</br>
Pipelines & Graphs [Hands-on]</br>
Experiments [Hands-on]</br>
Model groups [Hands-on]</br>
Endpoints [Hands-on]</br>



