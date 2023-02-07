---
layout: default
title: Linux Quick Installation
nav_order: 1
nav_exclude: true
parent: Linux
grand_parent: PC
---


## Quick Installation 

---

The quick-installation option saves time and labour, and is less error prone than manual installation. It helps you set up a running environment of formsflow.ai by installing the necessary packages and customizing the configuration files automatically. 


### Prerequisites

- For installation of formsflow.ai, the [Docker Desktop](https://www.docker.com/) needs to be installed . If Docker has been installed, and if any previous formsflow.ai installations were done already, those need to be removed from the Docker Desktop.  



## Steps for formsflow.ai Installation  

1.Download the following installation bundle to perform Quick Installation
  
<span class="fs-5">
[Formsflow.ai_windows-zip](https://github.com/AOT-Technologies/forms-flow-ai-deployment/archive/refs/heads/main.zip){: .btn .btn-purple .mr-4}
</span>   

2.Extract the contents of the downloaded zip file in the desired location   

3.Open the Extracted folder, choose the folder forms-flow-ai-deployment and then open the folder scripts

  ![folder](../../../assets/QuickDocker/quickfolder.png)
  
4.Double click on the install.bat file for quick Installation 

 ![install](../../../assets/QuickDocker/install_batchfile.png)
  {: .mt-6 .ml-6}

5.The installation starts with the following question,

 ![installqstn1](../../../assets/QuickDocker/runscript1.png)
  {: .mt-6 .ml-6}  

  *a*.  If you need Redash Analytics Engine in the installation, provide ‘y’ as the answer, or else answer ‘n’. (To know more about Redash Analytics Engine, please visit [Redash](https://redash.io/help/) ).  
 {: .ml-5}

 ![installqstn2](../../../assets/QuickDocker/runscript2.png)
 {: .mt-6 .ml-6}  
  *b*. Verify the IP address is valid or incorrect after that. If true, provide  'y' as the answer, or else answer ‘n’.    
  {: .ml-5}
 ![installqstn3](../../../assets/QuickDocker/runscript3.png)  
  {: .mt-6 .ml-6}    
 *c*. Provide the proper ip address.
 {: .ml-5}

6.As part of the installation, if the user has chosen the option to install with “Analytics” the user is asked to enter the Redash API key after the successful installation of Redash.  

 ![install](../../../assets/QuickDocker/apikey.png)
  {: .mt-6 .ml-6} 

7.The Redash application should be available for use at port defaulted to 7000. Open [http://localhost:7000/](http://localhost:7000/) on your machine and register with any valid credentials.

 ![install](../../../assets/QuickDocker/redash.png)
  {: .mt-6 .ml-6} 

8.To get the Redash API key, log in to [http://localhost:7000/](http://localhost:7000/),Choose Settings>>Account, and copy the API Key.

 ![install](../../../assets/QuickDocker/redashapikey.png)
  {: .mt-6 .ml-6} 

9.Copy the API Key and paste it into the cmd. The installation will continue.  

10.Once the installation is complete, the command prompt displays the installation is complete. The Docker Desktop displays all the installed containers.  

11.Health check can be applied.  





---





  *Copyright© [formsflow.ai](https://formsflow.ai/)*   
  {: .text-center .mt-8 .pt-8}