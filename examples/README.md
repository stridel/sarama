# Sarama examples

This folder contains example applications to demonstrate the use of Sarama. For code snippet examples on how to use the different types in Sarama, see [Sarama's API documentation on godoc.org](https://godoc.org/github.com/Shopify/sarama)

In these examples, we use `github.com/Shopify/sarama` as import path. We do this to ensure all the examples are up to date with the latest changes in Sarama. For your own applications, you may want to use `gopkg.in/Shopify/sarama.v1` to lock into a stable API version.

#### HTTP server

[http_server](./http_server) is a simple HTTP server uses both the sync producer to produce data as part of the request handling cycle, as well as the async producer to maintain an access log. It also uses the [mocks subpackage](https://godoc.org/github.com/Shopify/sarama/mocks) to test both.

#### SASL SCRAM Authentication
[sasl_scram_authentication](./sasl_scram_authentication) is an example of how to authenticate to a Kafka cluster using SASL SCRAM-SHA-256 or SCRAM-SHA-512 mechanisms.
