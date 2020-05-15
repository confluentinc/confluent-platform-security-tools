Confluent Platform Security Tools
=================================

This repo contains a tool that generates Kafka keystores and trust stores, along with a diagram that explains how keystores and trust stores can be deployed in Kafka.

Both the diagram and the script store the CA in the trust store. The trust store can be configured in other ways, for example, with multiple CAs, or with certificates instead of CAs. However, at this time, the diagram and the script don't address these additional configurations.

## User-input vs. Scripted Installation

- `kafka-generate-ssl.sh` - asks for user input
- `kafka-generate-ssl-automatic.sh` - scripted installation, requires these environment variables to be set (example):
  - `COUNTRY`
  - `STATE`
  - `ORGANIZATION_UNIT`
  - `CITY`
  - `PASSWORD`

Example:
```
export COUNTRY=US
export STATE=IL
export ORGANIZATION_UNIT=SE
export CITY=Chicago
export PASSWORD=secret
bash ./kafka-generate-ssl-automatic.sh
```
