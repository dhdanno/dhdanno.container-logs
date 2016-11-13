# dhdanno.container-logs
Enables container logging for a compose service via tail > file.log

The advantages writing the logs out to file over simply using gelf from the compose file are that with only UDP support we might loose logs, we cant view the logs on the server retrospectively and we lose multiline support which we could get from filebeat tailing the log.

### What does it do?
Should also interact with a filebeat role to install filebeat and place a config file for the designated log
