# What is Kafka?

In summary, we can say **Apache Kafka** is a **message broker**.

It's a highly scalable, and distributed platform for creating and processing streams in real-time.

Kafka broker is a middle man between producers and consumers.

In a more elaborate answer, we can say **Apache Kafka** is a horizontally scalable, fault-tolerant, distributed streaming platform.

## Broker Resposabilities:

1. Receive message from the producers and acknowledge the sucessful receipt.
2. Store the messages in a log file to safeguard it from potential loss.
3. Deliver the messages to the consumers when they request it.

