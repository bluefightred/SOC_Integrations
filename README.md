# SOC_Integrations
Sharing of enhanced Wazuh TheHive integrations, as well as a working SOC docker-compose configuration.

## 1. Docker-Compose file

The docker-compose published contains of:
  1. TheHive
  2. MISP 
  3. Cortex 
  4. Cassandra
  5. Elasticsearch
  6. Minio
  7. My_SQL (used by MISP)
  8. Portainer (optional)
  9. webhook (optional, used for Slack Notification)

Please feel free to change configurations according to your actual environment and deployment. e.g. Port numbers used by varies SOC instances.

## 2. Enhnaced Wazuh and TheHive integration script

The Wazuh and TheHive integration script shared here is an enhanced version of the orginal version published on the [Wazuh website](https://wazuh.com/blog/using-wazuh-and-thehive-for-threat-protection-and-incident-response/). 

Major enhancement included:
  1. Enhanced error handling throughout
  2. More comprehensive artifact mapping
  3. Better logging with more context
  4. Proper enumeration usage for severity, status, TLP, and PAP
  5. More robust timestamp handling
  6. Better tag management
  7. Future-proof type handling

NOTE: 
To use TheHive V5
```
pip install "thehive4py==2.0.0b6"
```


