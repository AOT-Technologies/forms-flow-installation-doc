---
layout: default
title: On Windows 
nav_order: 1
nav_exclude: true
---

## Windows install

#### Table of contents
1. <a href="/Pages/quickinstallation/onWindows.html#quick-installation" >Quick installation</a> 
2. More Installation Methods 
  - <a href="/Pages/Docker_Based/DockerFull.html" >Docker Full deployment</a>
  - <a href="/Pages/Docker_Based/IndividualService.html">Individual service deployment</a>


---

### System requirements
 
- 64-bit with at least 16GB RAM and 25GB HDD  
- This installation is supported only by Node.js versions 14 and below 

## Quick installation 

---

The quick-installation option saves time and labour, and is less error prone than manual installation. It helps you set up a running environment of formsflow.ai by installing the necessary packages and customizing the configuration files automatically. 


### Prerequisites

1. For installation of formsflow.ai, the [Docker Desktop](https://www.docker.com/) needs to be installed . If Docker has been installed, and if any previous formsflow.ai installations were done already, those need to be removed from the Docker Desktop.  


2. This installation is supported only by Node.js versions 14 and below (older versions of Node.js are listed [here](https://nodejs.org/en/download/releases/)).  

## Steps for formsflow.ai Installation  

1.Download the following installation bundle to perform Quick Installation
  
<span class="fs-8">
[Formsflow.ai_windows-zip](https://github.com/AOT-Technologies/forms-flow-ai-deployment/archive/refs/heads/main.zip){: .btn .btn-green .mr-4}
</span>   

2.Extract the contents of the downloaded zip file in the desired location   

3.Open the Extracted folder, choose the folder forms-flow-ai-deployment and then open the folder scripts

  ![folder](../../assets/QuickDocker/quickfolder.png)
  
4.Double click on the install.bat file for quick Installation 

 ![install](../../assets/QuickDocker/install_batchfile.png)
  {: .mt-6 .ml-6}

5.The installation starts with the following question,

 ![installqstn1](../../assets/QuickDocker/runscript1.png)
  {: .mt-6 .ml-6}  

  *a*.  If you need Redash Analytics Engine in the installation, provide ‘y’ as the answer, or else answer ‘n’. (To know more about Redash Analytics Engine, please visit [Redash](https://redash.io/help/) ).  
 {: .ml-5}

 ![installqstn2](../../assets/QuickDocker/runscript2.png)
 {: .mt-6 .ml-6}  
  *b*. Verify the IP address is valid or incorrect after that. If true, provide  'y' as the answer, or else answer ‘n’.    
  {: .ml-5}
 ![installqstn3](../../assets/QuickDocker/runscript3.png)  
  {: .mt-6 .ml-6}    
 *c*. Provide the proper ip address.
 {: .ml-5}

6.As part of the installation, if the user has chosen the option to install with “Analytics” the user is asked to enter the Redash API key after the successful installation of Redash.  

 ![install](../../assets/QuickDocker/apikey.png)
  {: .mt-6 .ml-6} 

7.The Redash application should be available for use at port defaulted to 7000. Open [http://localhost:7000/](http://localhost:7000/) on your machine and register with any valid credentials.

 ![install](../../assets/QuickDocker/redash.png)
  {: .mt-6 .ml-6} 

8.To get the Redash API key, log in to [http://localhost:7000/](http://localhost:7000/),Choose Settings>>Account, and copy the API Key.

 ![install](../../assets/QuickDocker/redashapikey.png)
  {: .mt-6 .ml-6} 

9.Copy the API Key and paste it into the cmd. The installation will continue.  

10.Once the installation is complete, the command prompt displays the installation is complete. The Docker Desktop displays all the installed containers.  

11.Health check can be applied.  

### Health Check  

- Analytics should be up and available for use at port defaulted to 7000 i.e. [http://localhost:7000/](http://localhost:7000/).
- Business Process Engine should be up and available for use at port defaulted to 8000 i.e. [http://localhost:8000/camunda/](http://localhost:8000/camunda/).

- FormIO should be up and available for use at port defaulted to 3001 i.e. [ http://localhost:3001/checkpoint]( http://localhost:3001/checkpoint).
- formsflow.ai REST API should be up and available for use at port defaulted to 5000 i.e. [http://localhost:5000/checkpoint](http://localhost:5000/checkpoint).
- formsflow.ai web application should be up and available for use at port defaulted to 3000 i.e. [http://localhost:3000/](http://localhost:3000/). 
- Default user credentials are provided  <a href="/Pages/user_credentials.html" target="_blank">here</a>.



---

  *Copyright© [formsflow.ai](https://formsflow.ai/)*   
  {: .text-center .mt-8 .pt-8}