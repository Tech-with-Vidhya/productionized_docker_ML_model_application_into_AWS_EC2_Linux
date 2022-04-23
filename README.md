# productionized_docker_ML_model_application_into_AWS_EC2_Linux

This project covers the end to end implementation of deploying and productionizing a dockerized/containerized machine learning python flask application into AWS Elastic Compute Cloud (EC2) Instance and AWS Elastic Container Registry (ECR) Service.  

The machine learning business case implemented in this project includes a bank note authentication binary classifier model using Random Forest Classifier; which predicts and classifies a bank note either as a Fake Bank Note (Label 0) or a Genuine Bank Note (Label 1).  

Project Architecture:

![](architecture/project_architecture.jpg)

Implementation Steps:

1. Creation of an end to end machine learning solution covering all the ML life-cycle steps of Data Exploration, Feature Selection, Model Training, Model Validation and Model Testing on the unseen production data. 
2. Saved the finalised model as a pickle file. 
3. Creation of a Python Flask based API; in order to render the ML model solution and inferences to the end-users. 
4. Verified and tested the working status of the Python Flask API in the localhost set-up. 
5. Creation of a Docker File (containing the steps/instructions to create a docker image) for the Python Flask based Bank Note Authentication Machine Learning Application embedded with Random Forest ML Classifier Model.
6. Creation of IAM Service Roles with appropriate policies to access the AWS Elastic Container Registry (ECR) Service and AWS Elastic Compute Cloud (EC2) Service. 
7. Created a new EC2 Linux Server Instance in AWS and copied the web application project’s directories and its files into the AWS Linux Server using SFTP linux commands. 
8. Installed the Docker software and the supporting python libraries in the AWS EC2 Linux Server Instance; as per the “requirements.txt” file. 
9. Transformation of the Docker File into a Docker Image and Docker Container representing the application; using docker build and run commands. 
10. Creation of a Docker Repository within the AWS ECR Service and pushed the application docker image into the repository using AWS Command Line Interface (CLI) commands. 
11. Deployment of the dockerized/containerized Python Flask ML application into the AWS EC2 Linux Instance; with the creation of the production end-point. 
12. Verified and tested the inferences of the productionized ML Application using the AWS EC2 end-point.  


Tools & Technologies:

1. Python
2. Flask
3. AWS
4. AWS EC2
5. Linux Server
6. Linux Commands
7. Command Line Interface (CLI)
8. Docker
9. Docker Commands
10. AWS ECR
11. AWS IAM


