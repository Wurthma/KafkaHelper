# Kafka simple project with Producer & Consumer

This project is based on confluent's "get-started" documentation and serves as a reference base for simple projects.

For more details, access the documentation or specific projects of the **Producer** and **Consumer**.


Both projects depend on installing the Confluent.Kafka package:

`dotnet add package Confluent.Kafka`

Other packages installation:

`dotnet add package Microsoft.Extensions.Configuration`

`dotnet add package Microsoft.Extensions.Configuration.Ini`

## Before running

Before running the application it is necessary to create the file 'getting-started.properties' in the project root. This file will be sent as an argument when running the application, but if you want you can change this format to use a secret or other formats.

### getting-started.properties content

```
bootstrap.servers=cluster-id.region.provider.confluent.cloud:9092
security.protocol=SASL_SSL
sasl.mechanisms=PLAIN
sasl.username=< CLUSTER API KEY >
sasl.password=< CLUSTER API SECRET >
```

## Produce events

To run the Producer application, run the command below:

`dotnet run --project .\producer.csproj  <PROJECT_PATH>\getting-started.properties`

## Consume events

To run the Consumer application, run the command below:

`dotnet run --project .\consumer.csproj  <PROJECT_PATH>\getting-started.properties`