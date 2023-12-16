# flask_5_tailwind

## 1. Video Creation or Procurement:
I have chosen a 1 minute video of Public service announcement (PSA) on Mental Health 

## 2. Cloud CDN & Video Hosting:
For this assignment I created a cloud CDN in Azure by following the steps mentioned below:

1. Sign in Azure.
2. Go to Storage Accounts and create a new storage account.
3. Go to Overview and click on Security. Enable the following:
    Secure transfer required
    Allow Blob anonymous access
    Allow storage account key access
4. Go to Containers and create a new container. Set the access level to Container (anonymous read access for containers and blobs).
5. Go into the new container and upload the video file.
6. Go to Front Door and CDN and create a new endpoint using the following configurations:
   Service type: Azure CDN
    Query string caching behavior: Ignore query strings
7. Once the endpoint is deployed, click on click an open a new tab using the endpoint hostname link.
8. In the first tab, go back to Containers and click on the container you created earlier. Then, click on the video file url and copy everything after .net/.
9. Go back to the new tab opened in step 7 and paste the url after .net/. The video should now be displayed on the page. Copy this url as it will be used in the index.html file.

## Deploying Flask App to Azure App Service 
1. Open up Google Cloud Shell.
2. Clone the repository using git clone and cd into the repository. Then design the flask app.
3. Add a requirements.txt file using pip freeze > requirements.txt.
4. In the terminal, run curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash to install Azure CLI.`
5. Run az login and follow the instructions to login to Azure.
6. Run az webapp up --resource-group <resource-group> --name <app-name> --runtime PYTHON:3.9 --sku B1 to deploy the app to Azure App Service. Replace <resource-group> with the resource group name and <app-name> with the app name.
7. After the deployment, go to Azure and click on App Services. Then, click on the app you just deployed and click on the the link under Default domain. The app should now be displayed on the page.

