# Kafka Inbound Endpoint

Kafka inbound endpoint acts as a message consumer. It creates a connection to ZooKeeper and requests messages for a topic.

## Compatibility

| Inbound Endpoint version                                                                                  | Supported Kafka version | Supported WSO2 ESB/EI version            |
|-----------------------------------------------------------------------------------------------------------|-------------------------|------------------------------------------|
| [1.0.113](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.10) | 2.13-3.6.1               | EI 6.5.0  , MI 4.2.0                     |
| [1.0.10](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.10)  | 2.12-2.2.1              | EI 6.1.1, EI 6.4.0, EI 6.5.0  , MI 1.1.0 |
| [1.0.9](https://github.com/wso2-extensions/esb-inbound-kafka/tree/v1.0.9)                                 | 2.12-2.2.1              | EI 6.1.1, EI 6.4.0, EI 6.5.0  , MI 1.1.0 |
| [1.0.8](https://github.com/wso2-extensions/esb-inbound-kafka/tree/v1.0.8)                                 | 2.12-2.2.1              | EI 6.1.1, EI 6.4.0, EI 6.5.0  , MI 1.1.0 |
| [1.0.7](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.7)    | 2.12-2.2.1              | EI 6.1.1, EI 6.4.0, EI 6.5.0             |
| [1.0.6](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.6)    | 2.12-1.0.0              | EI 6.1.1, EI 6.4.0, EI 6.5.0             |
| [1.0.5](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.5)    | 2.12-1.0.0              | EI 6.2.0, ESB 4.9.0                      |
| [1.0.4](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.4)    | 2.12-1.0.0              | EI 6.2.0, ESB 4.9.0                      |
| [1.0.3](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.3)    | 2.12-1.0.0              | EI 6.2.0, ESB 4.9.0                      |
| [1.0.2](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.2)    | 2.12-1.0.0              | ESB 4.9.0                                |
| [1.0.1](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.1)    | 2.12-1.0.0              | ESB 4.9.0                                |
| [1.0.0](https://github.com/wso2-extensions/esb-inbound-kafka/tree/org.apache.synapse.kafka.poll-1.0.0)    | 2.12-1.0.0              | EI 6.1.1, ESB 4.9.0, ESB 5.0.0           |

## Getting started

To get started with the inbound endpoint, go to [Configuring Kafka Inbound Endpoint](docs/config.md). Once you have completed your configurations, you can consume the messages that are produced by the kafka producer via a topic.   

## Building from the source

Follow the steps given below to build the Kafka Inbound Endpoint from the source code.

1. Get a clone or download the source from [Github](https://github.com/wso2-extensions/esb-inbound-kafka).
2. Run the following Maven command from the `wso2mi-kafka-inbound-endpoint` directory: `mvn clean install`.
3. The JAR file for the Kafka Inbound Endpoint is created in the `wso2mi-kafka-inbound-endpoint/target` directory.
4. The dependencies are copied to `target/connector/dependencies`


## How to use

1. Copy all above dependencies to `${MI_HOME}/lib`
2. Copy JAR file of the inbound endpoint to `${MI_HOME}/dropins`
3. Start the Micro Integrator by `bash ${MI_HOME}/bin/micro-integrator.sh`