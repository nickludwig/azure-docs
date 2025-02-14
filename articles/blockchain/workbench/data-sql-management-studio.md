---
title: Query Azure Blockchain Workbench data using SQL Server Management Studio
description: Learn how to connect to Azure Blockchain Workbench's SQL Database from within SQL Server Management Studio.
ms.date: 02/18/2022
ms.topic: how-to
ms.service: azure-blockchain
ms.reviewer: mmercuri
#Customer intent: As a developer, I want to use SQL Server Management Studio to query Azure Blockchain Workbench data.
---
# Using Azure Blockchain Workbench data with SQL Server Management Studio

[!INCLUDE [Retirement note](./includes/retire.md)]

Microsoft SQL Server Management Studio provides the ability to rapidly
write and test queries against Azure Blockchain Workbench's SQL DB. This section contains a step-by-step walkthrough of how to connect to Azure Blockchain Workbench's SQL Database from within SQL Server Management Studio.

## Prerequisites

* Download [SQL Server Management Studio](/sql/ssms/download-sql-server-management-studio-ssms).

## Connecting SQL Server Management Studio to data in Azure Blockchain Workbench

1. Open the SQL Server Management Studio and select **Connect**.
2. Select **Database Engine**.

    ![Database engine](./media/data-sql-management-studio/database-engine.png)

3. In the **Connect to Server** dialog, enter the server name and your
   database credentials.

    If you are using the credentials created by the Azure Blockchain Workbench deployment process, the username is **dbadmin** and the password is the one you provided during deployment.

    ![Enter SQL credentials](./media/data-sql-management-studio/sql-creds.png)

   1. SQL Server Management Studio displays the list of databases, database views, and stored procedures in the Azure Blockchain Workbench database.

      ![Database list](./media/data-sql-management-studio/db-list.png)

5. To view the data associated with any of the database views, you can automatically generate a select statement using the following steps.
6. Right-click any of the database views in the Object Explorer.
7. Select **Script View as**.
8. Choose **SELECT to**.
9. Select **New Query Editor Window**.
10. A new query can be created by selecting **New Query**.

## Next steps

> [!div class="nextstepaction"]
> [Database views in Azure Blockchain Workbench](database-views.md)
