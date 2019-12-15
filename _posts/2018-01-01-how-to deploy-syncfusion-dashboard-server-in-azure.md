---
title: How to deploy Syncfusion Dashboard Server in Azure?
author: arasu_rrk
show_comments: true
permalink: "/blog/how-to deploy-syncfusion-dashboard-server-in-azure"
categories: [ Syncfusion, Dashboard Server ]
image: images/blog-hero/syncfusion-dashboard-platform.png
tags: [syncfusion, dashboard-server, azure]
redirect_from:
  - /syncfusion/2018/01/01/how-to deploy-syncfusion-dashboard-server-in-azure/
---

We have simplied the Syncfusion Dashboard Server deployment in Azure. All you need is purchase a new virtual machine in Azure and Syncfusion Dashboard Server works with lowset plan too.

1. Login into [Azure Portal](https://portal.azure.com) with your credentials

2. Go to New and search the keyword `Syncfusion`. From the search results, select the `Syncfusion Dashboard Server` and proceed to create.
   ![](/images/dashboard-server/azure-deployment/syncfusion-dashboard-server-azure-search.png)
   ![](/images/dashboard-server/azure-deployment/syncfusion-dashboard-server-azure-create.png)
   
3. From the next screen, create the credentials for your Virtual Machine. If you want to use any existing resource group, choose the xisting one or create a new resource group.
   ![](/images/dashboard-server/azure-deployment/create-azure-vm-credentials.png)
   
4. Select the VM plan based on your requirements. 
   ![](/images/dashboard-server/azure-deployment/azure-vm-plans.png)
   
5. In the next step, disable the Boot diagnostics and use default settings for other options.
   ![](/images/dashboard-server/azure-deployment/azure-vm-optional-configuration.png)
   
6. In the last step, view the VM summary and proceed to create the VM.
   
   
That's all. It will take some minutes to complete the deployment and you can use Syncfusion Dashboard Server once it deployed.

<iframe width="100%" height="500" src="https://www.youtube.com/embed/eD7M_UN-COE" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>