# Kappa Architecture Sample

### Verify topics:

```
# In different command line windows ...

docker-compose -f kafka.yml exec broker kafka-console-consumer --bootstrap-server broker:9092 --from-beginning --property print.key=true --topic transaction_input

docker-compose -f kafka.yml exec broker kafka-console-consumer --bootstrap-server broker:9092 --from-beginning --property print.key=true --topic transaction_output

docker-compose -f kafka.yml exec broker kafka-console-consumer --bootstrap-server broker:9092 --from-beginning --property print.key=true --topic summary_output
```     

### TODO
1. Ingest Avro `timestamp` to Postgres `Timestamp`

