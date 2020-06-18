# Logstash Configurations


## pfsense.conf

This logstash file currently only handles the firewall logs, and does not conform to the ECS.

To configure pfsense:

Go to the Syslog configuration page: ``Status -> System Logs -> Settings -> Remote Logging Options``

Ensure **Enable Remote Logging** -> **Send log messages to remote syslog server** is checked

Ensure one of the **Remote log servers** is your logstash node.

Enable **Remote Syslog Contents** -> **Firewall Events**