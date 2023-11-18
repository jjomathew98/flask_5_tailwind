# flask_5_tailwind

## 1. Video Creation or Procurement:
#### I have chosen a 1 minute video of Public service announcement (PSA) on Mental Health 

## 2. Cloud CDN & Video Hosting:
#### For this assignment I created a cloud CDN in Azure by following the steps mentioned below:

##### a. Sign in Azure with credentials
##### b. Search s<mark>storage account</mark>
##### c. click create
##### d. Select subscription and resource group we would keep all other settings to be the same, we create Storage account name and press create
under overview, click on Security, Make sure Secure transfer required, Allow Blob anonymous access, and Allow storage account key access are enabled
Under data storage, click containers
Click + containers, change anonymous access level to container(anonymous read access for containers and blob) and create a name
Under Security + networking click Front Door and CDN
Under service type, click Azure CDN, create new, profile name, endpoint name
Under Query string caching behavior click Ignore Query String, press create
Click on the name and press upload a video of choice that is less than 60 seconds
Click on the video and copy the URL into a new tab to show that the video works.
Using the endpoint username URL, copy everything after the .net from the video link. This link would be the outcome
