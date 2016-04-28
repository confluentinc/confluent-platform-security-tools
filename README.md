Confluent Platform Security Tools
=================================

This repo contains a tool that generates Kafka keystores and trust stores, along with a diagram that explains how keystores and trust stores can be deployed in Kafka.

Both the diagram and the script store the CA in the trust store. The trust store can be configured in other ways, for example, with multiple CAs, or with certificates instead of CAs. However, at this time, the diagram and the script don't address these additional configurations.
