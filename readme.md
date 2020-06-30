# Configurações do cassandra

## Imagem docker

https://hub.docker.com/_/cassandra

## Como conectar no cassandra pela linha de comando - **DOCKER**
docker run -it --network cassandra_cass-network --rm cassandra cqlsh cassandra_cassandra_1


## Ver todos os keyspaces
```
SELECT * FROM system_schema.keyspaces
```

## Ver todos as tabelas 
```
describe tables;
```

## Ver todos as tabelas de um Keyspace
```
SELECT * FROM system_schema.tables WHERE keyspace_name = 'system_auth';
```