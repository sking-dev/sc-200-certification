# Exam Skill 3: Mitigate Threats Using Azure Sentinel (40-45%)

## 3A: Design and Configure an Azure Sentinel Workspace

- Plan an Azure Sentinel workspace
- Configure Azure Sentinel roles
- Design Azure Sentinel data storage
- Configure Azure Sentinel service security

----

## 3B: Plan and Implement the Use of Data Connectors for Ingestion of Data Sources in Azure Sentinel

- Identify data sources to be ingested for Azure Sentinel
- Identify the prerequisites for a data connector
- Configure and use Azure Sentinel data connectors
  - Microsoft 365
    - Microsoft Defender for Endpoint
    - Microsoft Defender for Identity
    - Microsoft Defender for Office 365
    - Microsoft Cloud App Security
  - Azure and Microsoft-related services
    - Azure Active Directory 
      - Audit logs
      - Sign-in logs
    - Azure Activity
    - Azure AD Identity Protection
    - Azure DDoS Protection
    - Azure Defender for IoT
      - Formerly "Azure Security Center for IoT"
    - Azure Information Protection
    - Azure Firewall
    - Azure Security Center
      - Alerts from Azure Defender solutions
    - Azure Web Application Firewall (WAF)
      - Formerly "Microsoft WAF"
    - Cloud App Security
    - Domain name server
    - Office 365
    - Windows firewall
    - Security Events
  - Third-party specific
    - CEF (Common Event Format)
    - Syslog
    - Custom connectors using the Log Analytics API
    - Logstash plugin
- Design Syslog and CEF collections
  - Choose CEF wherever possible
    - Format is easier to process
      - **Parsed** versus unparsed
  - Connect the CEF or Syslog Collector to Azure Sentinel
    - Agent must deploy on a dedicated Azure virtual machine (VM) or an on-premises system to support the appliance's communication with Azure Sentinel
    - You can deploy the agent automatically or manually
      - Automatic deployment is only available if your dedicated machine is a Virtual Machine in Azure
- Design and Configure Windows Events collections
- Configure custom threat intelligence connectors
- Create custom logs in Azure Log Analytics to store custom data

----

## 3C: Manage Azure Sentinel Analytics Rules

- Design and configure analytics rules
- Create custom analytics rules to detect threats
- Activate Microsoft security analytical rules
- Configure connector provided scheduled queries
- Configure custom scheduled queries
- Define incident creation logic

----

## 3D: Configure Security Orchestration Automation and Remediation (SOAR) in Azure Sentinel

- Create Azure Sentinel playbooks
- Configure rules and incidents to trigger playbooks
- Use playbooks to remediate threats
- Use playbooks to manage incidents
- Use playbooks across Microsoft Defender solutions

----

## 3E: Manage Azure Sentinel Incidents

- Investigate incidents in Azure Sentinel
- Triage incidents in Azure Sentinel
- Respond to incidents in Azure Sentinel
- Investigate multi-workspace incidents
- Identify advanced threats with User and Entity Behaviour Analytics (UEBA)

----

## 3F: Use Azure Sentinel Workbooks to Analyze and Interpret Data

- Activate and customize Azure Sentinel workbook templates
- Create custom workbooks
- Configure advanced visualizations
- View and analyze Azure Sentinel data using workbooks
- Track incident metrics using the security operations efficiency workbook

----

## 3G: Hunt for Threats Using the Azure Sentinel Portal

- Create custom hunting queries
- Run hunting queries manually
- Monitor hunting queries by using Livestream
- Perform advanced hunting with notebooks
  - Two libraries available to simplify access to the Log Analytics data store via the standard API
    - Kqlmagic
      - Provides an easy to implement API wrapper to run KQL queries
    - msticpy
      - Microsoft Threat intelligence Python Security Tools
      - <https://msticpy.readthedocs.io/en/latest/>
  - A **Jupyter Notebook** allows you to create and share documents that contain live code, equations, visualizations, and explanatory text
    - Uses include data cleaning and transformation, numerical simulation, statistical modelling, machine learning, and much more!
    - Jupyter extends the scope of what you can do with Azure Sentinel data
      - Combines full programmability with a vast library collection for machine learning, visualization, and data analysis
      - These attributes make Jupyter a useful tool for security investigation and hunting
  - Several notebooks, developed by some of Microsoft's security analysts, are packaged with Azure Sentinel
    - Some of these notebooks are built for a specific scenario and can be used as-is
    - Others are samples intended to illustrate techniques and features that you can copy or adapt for use in your own notebooks
  - Other notebooks may also be imported from the Azure Sentinel Community GitHub
  - Notebooks have two components:
    - The **browser-based interface** where you enter and run queries and code and where the execution results are displayed
    - The **kernel** is responsible for parsing and executing the code itself
      - The Azure Sentinel notebook's kernel runs on an Azure virtual machine (VM)
  - <https://github.com/Azure/Azure-Sentinel-Notebooks/blob/8122bca32387d60a8ee9c058ead9d3ab8f4d61e6/A%20Getting%20Started%20Guide%20For%20Azure%20Sentinel%20ML%20Notebooks.ipynb>
- Track query results with bookmarks
- Use hunting bookmarks for data investigations
- Convert a hunting query to an analytical rule

----

## End of Exam Skill 3
