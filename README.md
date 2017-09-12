# Execution steps
1. In another terminal window download and start Artemis broker (tested with v2.1.0)
```
wget https://www.apache.org/dyn/closer.cgi?filename=activemq/activemq-artemis/2.1.0/apache-artemis-2.1.0-bin.zip&action=download
unzip apache-artemis-2.1.0-bin.zip
./apache-artemis-2.1.0/bin/artemis create ./artemis-broker
./artemis-broker/bin/artemis run
```
2. Back in an application terminal window make sure that host and port are correct in `src/main/resources/application.yml`
3. Execute application: `mvn clean spring-boot:run`
