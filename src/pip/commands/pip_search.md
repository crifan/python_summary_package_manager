# pip search

当想要安装某个库，但却又不知道该库的包名时，可以用：

```bash
pip search xxx
```

去数据源中查询有哪些相关的包。

## `pip search`举例

### kafka

```bash
[root@xxx-dev-01 exercise]# pip3 search kafka
kafka (1.3.5)                                     - Pure Python client for Apache Kafka
  INSTALLED: 1.3.5 (latest)
heroku-kafka (2.1.2)                              - Python kafka package for use with heroku's kafka.
pytest-kafka (0.3.1)                              - Zookeeper, Kafka server, and Kafka consumer fixtures for Pytest
kafka-utils (2.3.0)                               - Kafka management utils
chance-kafka (0.0.6)                              - The kafka library for chancefocus
dask-kafka (0.1.0.dev0)                           - Dask-Kafka reader
kafka-bundle (1.0)                                - Kafka support for applauncher
kafka-helper (0.2)                                - Makes it easy to use the kafka-python library with Apache Kafka on Heroku
scrapy-kafka (0.1.1)                              - Kafka-based components for Scrapy
kafka-connector (0.0.7)                           - A python module for communication with Kafka.
kafka-logger (0.3.0)                              - A simple Kafka logger in Python.
eventcore-kafka (0.3.3)                           - Produce and consume events with Kafka.
kafka-shell (0.1.1)                               - A supercharged, interactive Kafka shell built on top of the existing Kafka CLI tools.
kafka-quixey (0.9.0-q3)                           - Pure Python client for Apache Kafka
confluent-kafka (1.1.0)                           - Confluent's Python client for Apache Kafka
kafka-python (1.4.6)                              - Pure Python client for Apache Kafka
timi-kafka (0.0.2)                                - Pure Python client for Apache Kafka
kafka-scanner (0.3.4)                             - High Level Kafka Scanner, supporting inverse consuming and deduplication. Based on kafka-python library.
log-to-kafka (1.1.4)                              - log to kafka
sentry-kafka (1.1)                                - A Sentry extension which integrates with Apache Kafka.
kafka-rest (0.0.12)                               - Async client for Confluent's Kafka REST Proxy
kafka-tools (0.1.9)                               - A collection of tools and scripts for working with Apache Kafka
kafka-connect-python (0.0.3)                      - Kafka Connect Module
kafka-dev-tools (0.0.1)                           - Tools for Kafka developers
kafka-python-with-confluent-kafka (0.2)           - This python project use to consume/produce/manager the Kafka
aio-kafka-daemon (0.5.1)                          - Asynchronous Kafka Processing Daemon
scrapy-kafka-export (0.1.1)                       - Export Scrapy items to Kafka
kafka-rest-client (0.8.0)                         - A python kafka rest client
chatora.confluent-kafka-ext (0.3)                 - Apache Kafka and Schema Registry client libraries for Python on top of confluent-kafka-python.
kafka-utils-netease (1.4.9)                       - Easy way to use Kafka in python
stack-kafka-python (1.4.11)                       - Pure Python client for Apache Kafka
scrapy-kafka-redis (0.0.7)                        - Kafka and Redis based components for Scrapy.
kafka-splunk-connector (1.0.6)                    - Library that connects the kafka topic to splunk
confluent-kafka-helpers (0.7.3)                   - Helpers for Confluent's Kafka Python client
netbox-kafka-producer (1.0.10)                    - Easily publish NetBox changes to Kafka
gc-kafka-python (0.9.8)                           - Pure Python client for Apache Kafka
robinhood-kafka-python (1.4.3)                    - Pure Python client for Apache Kafka
kafka-connect-healthcheck (0.1.0)                 - A simple healthcheck wrapper to monitor Kafka Connect.
kafka-logging-handler (0.2.2)                     - A Python logging handler library for Kafka consumers.
netbox-kafka-consumer (1.0.6)                     - Easily consume NetBox changes from Kafka
heroku-kafka-eze (0.0.2)                          - Python kafka package for use with heroku's kafka. You'll only need your heroku api key and app name
logwatcher-kafka-plugin (1.0)                     - LogWatcher Plugin for Sending log lines to a Kafka Topic
python-elk-kafka (0.0.1)                          - A python3 elk project use kafka to send messages
confluent-kafka-smyte (0.9.3)                     - Smyte fork of Confluent's Apache Kafka client for Python
swissbib-kafka-event-hub (2.2.0)                  - Swissbib Kafka Event Hub
kafka-log-handler (1.2)                           - Simple python logging handler for forwarding logs to a kafka server.
python-kafka-logger (0.5)                         - Simple python logging handler for forwarding logs to a kafka server.
batching-kafka-consumer (0.0.4)                   - Kafka Consumer abstraction that assists with processing batches and committing offsets.
python-kafka-logging (0.6)                        - Simple python logging handler for forwarding logs to a kafka server.
reverse-kafka-logger (0.1.2)                      - grep kafka message reversely from the end offset to start offset
pipelinewise-tap-kafka (1.0.0)                    - Singer.io tap for extracting data from Kafka topic - PipelineWise compatible
ctodd-python-lib-kafka (1.0.2)                    - Python utilities used for interacting with Apache Kafka
kafka-avro-binary-consumer (0.0.0.2)              - Kafka avro binary consumer with postgres config
kafka-avro-producer-topkrabbensteam (1.3.1)       - Kafka (produce messages) using Apache Avro schemas
prometheus-kafka-consumer-group-exporter (0.5.1)  - Kafka consumer group Prometheus exporter
kafka-python-log-handler (0.0.1.dev12)            - A log handler for the Python logging module, emitting logs to Kafka topics.
kafka-metrics-producer-topkrabbensteam (1.0)      - Library that can be used to produce metrics to Kafka using Apache Avro schemas
gevent-kafka (0.2)                                - ApacheKafka bindings for gevent
kafka-cffi (0.11.4a5)                             - A CFFI binding for librdkafka
kafka-tfrx (0.14.0)                               - Add a short description here!
dox-kafka (0.0.1)                                 - 
kafka-transport (0.6.7)                           - 
ansible-runner-kafka (0.1)                        - 
kser-transport-kafka (0.1.0)                      - Kser librdkafka producer/consumer
samsa (0.3.11)                                    - Kafka Client for Kafka 0.7
azure-functions-kafka-binding (1.0.1)             - 
ickafka (0.1.4)                                   - improved colored kafka
esque (0.1.4a0)                                   - A usable kafka tool.
pysubman (1.20.1.4)                               - kafka simple using
zpython-tools (0.1.1)                             - kafka tools with python
kafkaloghandler (0.9.0)                           - Kafka Logging Handler
kafka_influxdb (0.9.3)                            - A Kafka consumer for InfluxDB
dhcpkit_kafka (1.0.0)                             - Kafka extensions to DHCPKit
robinhood-aiokafka (1.0.3)                        - Kafka integration with asyncio.
aiokafka (0.5.2)                                  - Kafka integration with asyncio.
kafkaBridgeClient (0.1.5)                         - A package for using kafka-bridge to talk to kafka inside docker
kafka_store (0.1.4)                               - Kafka Store provides an easy way of archiving data from Kafka
streamsx.kafka (1.2.4)                            - IBM Streams Kafka integration
kq (2.0.0)                                        - Kafka Job Queue for Python
fjord_kafka_migration (0.2.5)                     - fjord kafka migration tools.
kafkatos3 (0.2.0)                                 - Archive kafka messages to S3
bubuku (0.10.47)                                  - AWS support for kafka broker
xoskafka (3.3.1)                                  - Wrapper around kafka for XOS
robotframework-kafkalibrary (0.0.2)               - Kafka library for Robot Framework
kser (0.8.19)                                     - Kafka serialize python library
nico (0.1)                                        - job scheduler for kafka message
kafkaesque (1.0)                                  - an easy to use kafka consumer that extends kafka-python, but follows the style of the flask server
kiel (0.9.3)                                      - Kafka client for tornado async applications.
testing.kafka (0.0.1)                             - automatically setups a kafka instance for testing
kser-crypto (0.1.4)                               - Crypto Kafka serialize python library
yelp_kafka (5.2.1)                                - A library to interact with Apache Kafka at Yelp
kafkacrypto (0.9.4)                               - Message layer security/crypto for Kafka
asynckafka (0.1.2)                                - Fast python kafka client for asyncio.
kafka_replayer (1.0.1)                            - Timestamp-based Kafka topic replayer
robotframework-confluentkafkalibrary (0.3.0)      - Confluent Kafka library for Robot Framework
kafkacli (0.0.7)                                  - Apache Kafka CLI utility tool.
klag (1.0.2)                                      - A Kafka consumer group monitoring CLI.
Kafthon (0.0.1)                                   - High level Python wrapper for Kafka
afkak (3.0.0)                                     - Twisted Python client for Apache Kafka
flasfka (1.1.6)     
```

此处，找到我们希望安装的库是：

```bash
pip3 install kafka-python
```
