# udagramproject
Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

The project is split into three parts:

The Simple Frontend A basic Ionic client web application which consumes the RestAPI Backend. [Covered in the course]
The RestAPI Backend, a Node-Express server which can be deployed to a cloud service. [Covered in the course]
The Image Filtering Microservice, the final project for the course. It is a Node-Express application which runs a simple script to process images. [My assignment]
#Project Scope #@TODO1 IMPLEMENT A RESTFUL ENDPOINT My task was to create a REST API(Application Programming Interface ) endpoint that: // GETS /filteredimage?image_url={{URL}} // endpoint to filter an image from a public url.

// IT SHOULD
// 1. validate the image_url query // 2. call filterImageFromURL(image_url) to filter the image // 3. send the resulting file in the response // 4. delete any files on the server on finish of the response

QUERIES THE PARAMATERS // image_url: URL of a publicly accessible image for example: (https://upload.wikimedia.org/wikipedia/commons/b/bd/Golden_tabby_and_white_kitten_n01.jpg) AND // RETURNS // the filtered image file [ res.sendFile(filteredpath);

Completed Tasks
The code endpoint runs well and shows successful response code 200 ok.

1.All project code is stored in a GitHub repository and this link has been submitted for review. There are at least two branches - one for development (dev, development) and one master. Master should contain the most up-to-date, stable code at the time of submission.

2.The stubbed @TODO1 endpoint in src/server.ts is completed and accepts valid requests including: http://localhost:{{PORT}}/filteredimage?image_url=https://upload.wikimedia.org/wikipedia/commons/b/bd/Golden_tabby_and_white_kitten_n01.jpg

3.The project was deployed using the AWS Elastic Beanstalk CLI eb init, eb create, and eb deploy commands. A screenshot of the elastic beanstalk application dashboard is included in the deployment_screenshot directory.see EbDeploymentScreenshot file.

4.My endpoint URL below for the running elastic beanstalk deployment (EB_URL) has been submitted along with the project submission. Endpoint URL = http://imagefilterservice-dev.us-east-1.elasticbeanstalk.com

5.This endpoint responds to valid GET requests like: http://{{EB_URL}}/filteredimage?image_url=https://upload.wikimedia.org/wikipedia/commons/b/bd/Golden_tabby_and_white_kitten_n01.jpg that is:http://imagefilterservice-dev.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://upload.wikimedia.org/wikipedia/commons/b/bd/Golden_tabby_and_white_kitten_n01.jpg
