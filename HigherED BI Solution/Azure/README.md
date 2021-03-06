# Higher Education BI Solution - Azure 

Solutions needed to deploy BI to Azure:

00 - Environment Provisioning
* ARM template to provision Azure PaaS.
* Instructions to provision Azure PaaS using Azure Portal.
* [Optional] Instructions to provision Azure IaaS using Azure Portal.

01 - Data Validation
* Database Project to provision HigherED_Staging database.
* Integration Services Package to load HigherED_Staging database.
* Validation query to validate hackathon data load.

02 - Data Warehouse
* Database Project to provision HigherED_DW database.
* Post-execution script to grant access to Proxy user.

03 - SSIS ETL
* Integration Services Packages used to load HigherED_DW tables.
* DimDate table is loaded using stored procedure.
* T-SQL Script to modify HigherED_DW size, edition and service objective.

04 - SSAS Tabular
* Analysis Services Tabular model using HigherED_DW as data source.
* Deploy and process using SSMS.
* Some connectivity restrictions...

05 - SSRS Reporting
* Reporting Services Reports using HigherED_DW as data source.
* Enrollment Report with drillthrough to Enrollment Detail Report.
