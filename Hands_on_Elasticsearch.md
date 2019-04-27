# Instalar o Elasticsearch

## linux or mac:

```
tar -xzvf elasticsearch-6.7.1.tar.gz
cd elasticsearch-6.7.1
./bin/elasticsearch
```

## windows

Extraia o arquivo `elasticsearch-6.7.1.zip` e em seguida execute os comandos abaixo a partir do terminal.

```
cd C:\Program Files\elasticsearch-6.7.1
bin\elasticsearch.bat
```

Referência:
https://www.elastic.co/guide/en/elastic-stack-get-started/current/get-started-elastic-stack.html#install-elasticsearch

## Verifique

O Elasticsearch, por padrão, utiliza a porta 9200. Para verificar se ele está em execução acesso o seguinte endereço a partir do seu browser:

http://127.0.0.1:9200

Resultado esperado:

```
{
  "name" : "bPSmzCI",
  "cluster_name" : "elasticsearch",
  "cluster_uuid" : "m2a8rPoXS1Wx4vbmujBjPw",
  "version" : {
    "number" : "6.7.0",
    "build_flavor" : "default",
    "build_type" : "tar",
    "build_hash" : "8453f77",
    "build_date" : "2019-03-21T15:32:29.844721Z",
    "build_snapshot" : false,
    "lucene_version" : "7.7.0",
    "minimum_wire_compatibility_version" : "5.6.0",
    "minimum_index_compatibility_version" : "5.0.0"
  },
  "tagline" : "You Know, for Search"
}
```
