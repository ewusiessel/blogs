
In the field of cybersecurity, obtaining hands-on experience can be daunting due to the high cost of modern security defence utilities. However, I recently came across Wazuh - a Security Information and Event Management (SIEM) platform that is free, open source, easy to install and a ton of fun.  Wuzah seamlessly integates SIEM and Extended Detection and Response (XDR) solutions in a centralised location. This unified platform allows for effective management of security incidents and also incorporates Endpoint Detection and Response (EDR) capabilities. 
In this write-up I will be installing Wazuh on a main virtual machine as a host and  two virtual machines as agents while we explore its capabilities. This will be part one of a three part series for this project. 

## Brief History
Wuzah was started in 2015 as a fork of the OSSEC project. Wazuh is a private company incorporated in the United States. They are a team of about 190 people, distributed in about 12 different countries the majority of the team is in Argentina, Spain, and USA.
Wazuh Inc is registered in San Diego and has SOC2 and PCI-DSS compliance certifications.
Wazuh is a combination of 4x tools:

- Wazuh Indexer: OpenSearch fork which is an ElasticSearch fork.
- Wazuh Server: OSSEC fork
- Filebeat: From Elastic, ships the logs to OpenSearch
- Wazuh Dashboard: OpenSearch Dashboards fork which is a Kibana fork.

And because its's open source, you can also find the code on GitHub and audit or contribute to it yourself.

https://github.com/wazuh

## Documentation

