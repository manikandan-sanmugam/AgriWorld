# AgriWorld
This is our project for Future Ready Talent Internship program

This project is an agricultural website that helps agriculture business. It is deployed using Microsoft Azure Static Web Apps and includes downloadable catalog files that are stored in an Azure Storage account.

**Problem Statement/Opportunity:**

Online business websites are one of the ways to increase sales and income. As online business reduces the cost of physical requirements for a business. This project helps agricultural businesses to improve their sales and it makes customers easy to trade.

**Project Description:**

->Agriculture is the backbone of our country. Agriculture businesses are facing many challenges including losses due to stocking  products for a long time. 

->To speed up the rotation of goods, we are implementing websites to reach customers in other regions. 

->Customers can visit the website to explore the product availability and contact details of the retailer. 

->Specifications and description of each variety of crops are mentioned on the website itself to make it easier to select a variety.

->Customers can download a catalog of available products both in Excel and PDF format along with a product ID. 

->The section called "Request Call" asks for the mobile number of the customer to reach out easily. 

->This process reduces the cost due to physical requirements. 

->This project will help the agricultural business to be successful.



**Important Links**

Project Deployment link: https://proud-stone-09f058d10.2.azurestaticapps.net

Github Repository: https://github.com/manikandan-sanmugam/AgriWorld

Video Demonstration Link: https://youtu.be/DmuFWkKsnqo


**Team Members:**

1) Manikandan S : https://github.com/manikandan-sanmugam

2) Jeyaprakash J : https://github.com/JeyaprakashJp

3) Kaviyadevi M : https://github.com/kaviyadevi53

4) Koushika M : https://github.com/Koushika07


**1. Azure Services used and its features**

Azure Servies utilized:

a) Azure Static Web App
b) Azure Storage Accounts (container storage)

![Resources](https://user-images.githubusercontent.com/56933033/215108143-34aa84e2-920c-4f96-888d-b491e78a4f5a.png)


**1.1 Azure Static Web App**
     
AgriWorld project is deployed using Azure static web app services. Azure Static Web Apps is a service provided by Microsoft Azure that allows developers to host static web applications on Azure. A static web application is a website that consists of HTML, CSS, and JavaScript files that are served to the client without any server-side processing.

Some key features of Azure Static Web Apps include:

->Continuous deployment: Azure Static Web Apps automatically builds and deploys your website whenever you push changes to your code repository.

->Global scale: Azure Static Web Apps uses Azure's global network of datacenters to ensure that your website is delivered quickly and reliably to users around the world.

->Custom domains: You can use a custom domain for your website with Azure Static Web Apps.

->Security: Azure Static Web Apps includes built-in security features, such as TLS/SSL encryption, to help protect your website and its users.

**1.2 Azure Storage Account**

Azure Storage is a cloud-based service provided by Microsoft Azure that enables developers to store and manage data in the cloud. There are several types of storage options available, including:

->Blob storage: A service for storing large amounts of unstructured data, such as images, videos, and documents.

->File storage: A service for storing and sharing files, similar to a network file share.

->Table storage: A NoSQL key-value store for storing structured data at scale.

->Queue storage: A service for storing and retrieving messages in a queue, to enable communication between different parts of an application.

->Disk storage: A service for storing persistent disks that can be attached to Azure virtual machines.

**2. Deployment steps and implementation using Azure services**

**2.1 Deploy website using Azure static web app:**

->navigate to https://portal.azure.com/#create/Microsoft.StaticApp or click on new resource and then search for Azure Static Web App and click create.

->Select subscription, Resource group (agriworld), Name(agriworld) and Hosting plan.

->Select the source as github and then sign in with github account.

->Enter the project repository details.

->Then click review+create.

->Wait for deployement to complete.

**Deployment Screenshot (Azure Static Web App)**

![Azure static webapp](https://user-images.githubusercontent.com/56933033/215101866-2790c87d-9438-4cdd-b3e0-763e2514d977.png)



**2.2 Steps to upload files to container using the Azure portal:**

->Navigate to the Azure Storage account in the Azure portal or https://portal.azure.com/#create/Microsoft.StorageAccount-ARM.

->Create storage account resourse (agriworld). 

->Select the container (agriworld) in which we want to upload the file.

->Click the "Upload" button, then select the file(catalog) you want to upload.

->Once the file has been uploaded, it will be listed in the container.

->Set the container's access policies to public.

->The files are accessed through the public link.


Azure storage service is used for downloadable catalog. The files are uploaded to storage container named "agriworld".

**Azure Storage Account Screenshot (storage container name 'agriworld')**

![Azure storage account](https://user-images.githubusercontent.com/56933033/215102803-cfd645df-0f38-4553-8e60-06c6056b5b66.png)

**Azure Storage Container Screenshot that contains catalog files inside the 'agriworld' container that can be publicly accessed**
![Agriworld container (Storage account)](https://user-images.githubusercontent.com/56933033/215102979-797e053c-5974-4fdd-89ef-ce7a8c212ea8.png)

**Public Access link of catalog files**

PDF catalog: https://agriworld.blob.core.windows.net/agriworld/catalog.pdf

Excel catalog; https://agriworld.blob.core.windows.net/agriworld/catalog.xlsx

**Downloadable Catalog**

To download the catalog, users will need to have access to the container in Azure Storage. This can be done by providing them with a shared access signature (SAS) or by setting the container's access policies to public. The catalog is in formats which are Excel and PDF and it is uploaded in the container storage account.

This service is used to update the catalog in the website by just replacing the files in the azure storage container itself. This makes the process of catalog updation easier.

PDF catalog: https://agriworld.blob.core.windows.net/agriworld/catalog.pdf

Excel catalog; https://agriworld.blob.core.windows.net/agriworld/catalog.xlsx

The catalog can be downloaded by clicking download catalog buttons.

**(Screenshot)**


![Screenshot (2696)](https://user-images.githubusercontent.com/56933033/215105239-5eb605a5-658a-47ad-b794-7391713b3bed.png)


By clicking the Download, it will redirect to the catalog files uploaded in the azure storage accounts


![Screenshot (2697)](https://user-images.githubusercontent.com/56933033/215106682-6924e953-bdeb-4201-b98e-3e0f67e297da.png)





