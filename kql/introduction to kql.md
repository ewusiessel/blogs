This blog is about my dive into a data query language that has fascinated me since becoming a security analyst. KQL stands for Kusto Query Language, a data query language used primarily for security operations using Microsoft Azure and Microsoft 365 security and monitoring tools. Microsoft tools and platforms that primarily use KQL include: 

- Azure Data Explorer (ADX)
- Azure Log Analytics
- Microsoft Sentinel
- Azure Monitor
- Application Insights
- Microsoft 365 Defender

### Objectives
As KQL is such an extensive topic to learn, I have decided to break it down into small chunks or series for easy assimilation and retention, so for this blog my objectives are outlined as follows:

- Understanding the Fundamentals of KQL
- An overview of how KQL is used in security operations
- How to setup a free Azure Explorer environment
- Ingesting your data in Azure Explorer.


### Fundamentals of KQL
In cyber security KQL is used predominantly for log and event data analysis, monitoring performance, security analytics etc. In simple terms it allows users to extract insights from large amounts of data by writing queries. It is important to note that the Kusto Query Language is used for read-only requests to process data and return results. You would be unable to make modifications write data to tables or structure the columns. 

### Using KQL in Security Operations
Here are some examples of how KQL is used for querying and analysing data in security operations:

- **Log Analysis:** KQL provides security analysts with the ability to query and analyse log data from different sources including security event logs, network logs, application logs etc. Writing KQL queries will grant security teams the ability to search for specific security events, correlate different types of logs and uncover patterns, and identify suspicious activities or IOCs (Indicators of Compromise)  

- **Security Monitoring and Alerting:** used to customise and create security monitoring rules and alerts. In achieving this one would have to set continuous monitoring of critical security events by defining KQL - based queries that trigger alerts when specific conditions are detected. This helps in prompt identification and response to security incidents.

- **Threat Hunting**: KQL empowers security professionals to perform threat-hunting by scrutinising large volumes of data for indications of potential threats or malicious activities. This involves combining different data sources, applying filters and harnessing advanced analytics techniques. KQL queries can assist in identifying anomalies, discover sophisticated attack techniques and reveal hidden threats.

- **Security Analytics Platforms:** KQL is a fundamental component of security analytics platforms such as Microsoft Sentinel - a cloud-native SIEM and SOAR solutions. Microsoft Sentinel uses KQL as its query language for performing advanced log analytics threat detection and investigation. Security analysts with the help of KQL can build custom detection rules, generate reports and conduct crucial investigations.


### Setting up your Azure Explorer Environment
Now for the fun part, let's walk through the process of setting up how a free Azure Data Explorer environment. Head to 👉  https://dataexplorer.azure.com/  to create an account, you will need a Microsoft account for this purpose.

https://share.cleanshot.com/3QPxPxBs

The first task is to create a [cluster] and [data base]. To differentiate, a **cluster** is like a top-level container that holds everything together. It's where you manage and organise your data. Within a cluster, you can have one or more **databases**. Think of a database as a storage unit within the cluster where you store and organise specific sets of data. So, in simple terms, a cluster is like a big box that holds all your data, and databases are smaller boxes inside that big box where you keep different types of information organised.

https://share.cleanshot.com/K9YWnZ5S

### Ingesting your data in Azure Explorer
To ingest data into the database To add data head over to the My cluster menu option and select Action and Ingest data. You will be presented with four options to choose where to upload your data from. In this example my sample data is stored on my local computer so I chose option number 1. In the next part we will dive into writing our first query request. 

https://share.cleanshot.com/F11PjqQF