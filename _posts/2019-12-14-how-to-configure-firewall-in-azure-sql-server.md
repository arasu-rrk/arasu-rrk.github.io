---
title: How to configure firewall in Azure SQL Server?
categories:
  - azure-sql
author_staff_member: arasu_rrk
show_comments: true
---

Azure SQL Server is configured by default to connect to Azure Services alone. If you want to access the Azure SQL Server in your network you've to configure your IP address in Azure SQL Server Firewall.

1. Go to [https://portal.azure.com](https://portal.azure.com)

2. Navigate to your Azure SQL Server

3. From the navigation menu, select **Firewalls and virtual networks**

   ![](/images/azure/sql-server/azure-sql-firewall.png)

4. Configure your IP address in the page
   ![](/images/azure/sql-server/azure-sql-firewall-settings.png)


   a. Click **Add Client IP** option to allow your current IP address in the firewall. 

   b. Allow a particular IP address alone. For example 2.2.2.2. In this case, Start IP and End IP will be the same.

   c. You can allow the IP address range. For example 127.0.0.1 - 127.0.0.5. 

   d. You can either allow all IP addresses from 0.0.0.0 - 255.255.255.255.
      > If you enter these from to IP addresses, you can able to access the SQL Server from any IP address. But this is not preferable.

   e. Enable this option *Allow Azure services and resources to access this server* to allow your services that are hosted in Azure. 
      > NOTE: This option enables access to all services and resource (Not only your resources) that are hosted in Azure. 


5. Once you have configured IP addresses, click **Save** to save your changes.
