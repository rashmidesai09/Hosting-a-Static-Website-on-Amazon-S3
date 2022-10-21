# Hosting a Static Website on Amazon S3

## Project Goal 
Migrate an existing website to a static website on Amazon S3 in order to improve web application reliability
  1. Create an Amazon S3 bucket
  2. Enable static website hosting
  3. Secure Amazon S3 bucket using a bucket policy
  
### Diagram Steps
<img width="625" alt="image" src="https://user-images.githubusercontent.com/97893144/197002688-5a073408-44b4-4ef4-a94e-4891a0f3b277.png">
<img width="625" alt="image" src="https://user-images.githubusercontent.com/97893144/197002779-e0740ec0-5919-4f6f-bafd-9f2342d7af62.png">
<img width="625" alt="image" src="https://user-images.githubusercontent.com/97893144/197002877-3d0d290c-3499-4311-9b71-f9677b6718c4.png">
<img width="625" alt="image" src="https://user-images.githubusercontent.com/97893144/197002971-cffc8aa4-1f92-41f3-b788-2e3b23b10315.png">
<img width="625" alt="image" src="https://user-images.githubusercontent.com/97893144/197003109-4c8bee07-408b-4ee2-b407-412e9e6e3c25.png">
<img width="625" alt="image" src="https://user-images.githubusercontent.com/97893144/197003190-d6c52b48-52ff-4b26-965d-f1336369011c.png">
<img width="625" alt="image" src="https://user-images.githubusercontent.com/97893144/197003283-3256b455-0781-4e56-b447-a6ba0de4151d.png">
<img width="625" alt="image" src="https://user-images.githubusercontent.com/97893144/197003375-a2de2373-c64d-4d19-b738-85e3af11bfca.png">
<img width="625" alt="image" src="https://user-images.githubusercontent.com/97893144/196945808-eb9789eb-be6e-4421-968d-ec4d34cb330e.png">

### Files to be added to the bucket are listed below 
<img width="100" alt="image" src="https://user-images.githubusercontent.com/97893144/196934232-31c6621c-b494-4770-82a1-15c879531d9e.png">

### Steps mentioned below 

Step 1 : Go to the AWS console and click on S3 

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196934603-7ede87e1-dba6-4683-8bb4-cd263e09c85c.png">

The AWS Management Console is a web-based interface for accessing and managing AWS services. You can quickly access recently used services and search for other services by name, keyword, or acronym. The console includes wizards and automated workflows that can simplify the process of completing tasks.

Amazon S3 (Simple Storage Service) provides object storage, which is built for storing and recovering any amount of information or data from anywhere over the internet. It provides this storage through a web services interface.

Step 2: Create a bucket

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196935313-76771f48-5b67-49fc-8725-a2462510ed18.png">

A bucket is a container for objects stored in Amazon S3. You can store any number of objects in a bucket and can have up to 100 buckets in your account

Step 3: Give unique name for the bucket and follow the steps mentioned in screenshot

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196935795-1efb7a5d-e31f-4bdf-b15b-922ba6f9c160.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196935850-32c024ba-d24a-429f-bffd-7ba92952a644.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196935945-a4d541a8-2ea9-4ac8-a1fb-0de7fe7a8f6a.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196936063-10c038c9-a3a5-43b8-9288-baae6ed65caf.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196936292-c7586cd1-f98d-4d6e-b5c6-6ee0fab81c59.png">

Step 3: Click on the newly created bucket. In this case it is rashmisbucketforcloudquest and upload the data

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196936623-6c648958-30dd-4cd7-93e0-1ec5090fddbe.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196936701-6701b72e-c035-4d64-a343-8b2e652be31c.png">

Step 4: After adding file the final bucket would like below -

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196936826-a9c91e72-ad32-4be2-8b5d-5fb97e2f01ba.png">

Step 5 : Click on properties and scroll down to static website hosting and follow steps as mentioned in screenshot below

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196937779-d537d542-8f77-411a-9fdf-cc01a95a1e20.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196938003-cef78b63-4a47-4bee-9ac3-a3f4b1ba0ce3.png">

Note :

<img width="300" alt="image" src="https://user-images.githubusercontent.com/97893144/196938462-5e7dd015-d145-41d9-92ff-07285d476794.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196938610-5a0dd104-0838-4f7b-ad29-4471d7a8afc1.png">

Step 6 : Go to Permissions tab

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196938896-19f7c2fa-1811-4275-9aa3-d7e356f1fb0e.png">

Note :

<img width="300" alt="image" src="https://user-images.githubusercontent.com/97893144/196939024-78369cdc-10cb-45a4-9f61-84683b80e518.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196939085-97c48247-5905-4314-b02b-7d78f7a45c45.png">


Step 7 : Copy your buckets ARN, In this case the ARN is arn:aws:s3:::rashmisbucketforcloudquest

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196939372-9aa9f62f-1bf5-4e28-b4fb-4431a863acff.png">

Note :

<img width="300" alt="image" src="https://user-images.githubusercontent.com/97893144/196939575-56350953-67dc-42c3-b2dd-b028bf51964c.png">

Step 8 : Edit the policy and replace the ARN, ensure the ARN ends with /*

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196939943-50c297cb-cc7c-4da2-9803-4b4e82e94a99.png">

Follow the instructions else there will be error while saving

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196940648-ee4f79fa-47eb-49a5-a28e-5b6acce2aee2.png">

Step 9 : Save the changes as below 

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196940379-45ad1ae4-7d4d-4f20-9a55-125faca6afd5.png">

Step 10 : Go back to properties tab and scroll to static website hosting and follow the steps in screenshot

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196940930-db7e3771-bfed-4557-9242-869c65fa2740.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196940998-7b0ebb98-58ba-4a26-b179-0c79093cd1bc.png">

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196941232-4d404e70-3d15-477e-9ec4-73412e75d9f5.png">

This would like - http://rashmisbucketforcloudquest.s3-website-us-east-1.amazonaws.com

Note : 

<img width="300" alt="image" src="https://user-images.githubusercontent.com/97893144/196940873-2b63df8a-0143-4559-9bc8-afda2d9682ef.png">

Step 11 : Open a new window or browser tab with the new URL that was copied  - http://rashmisbucketforcloudquest.s3-website-us-east-1.amazonaws.com

The static website looks like below -

<img width="1000" alt="image" src="https://user-images.githubusercontent.com/97893144/196941535-c5dbc537-3d1d-493f-8b9d-de4f4492a85e.png">


Datasets source : Cloudquest AWS skillbuilder





