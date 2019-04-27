# Instalar o Kibana

## linux

```
tar xzvf kibana-6.7.1-linux-x86_64.tar.gz
cd kibana-6.7.1-linux-x86_64.tar.gz/
./bin/kibana
```

## mac:

```
tar xzvf kibana-6.7.1-darwin-x86_64.tar.gz
cd kibana-6.7.1-darwin-x86_64/
./bin/kibana
```

## windows

Extraia o arquivo `kibana-6.7.1-windows-x86_64.zip` e em seguida execute os comandos abaixo a partir do terminal.

```
cd C:\Program Files\kibana-6.7.1-windows
bin\kibana.bat
```

Referência:
https://www.elastic.co/guide/en/elastic-stack-get-started/6.7/get-started-elastic-stack.html#install-kibana

## Verifique

1. O Kibana, por padrão, utiliza a porta 5601. Para verificar se ele está em execução acesso o seguinte endereço a partir do seu browser:

http://127.0.0.1:5601

2. Em seguida acesso o [Dev Tools Console](http://localhost:5601/app/kibana#/dev_tools) a indexe um documento de exemplo:

```
PUT my_index/_doc/1
{
  "first_name": "John",
  "last_name": "Doe",
  "full_name": "John Joe Doe"
}
```

3. Vamos executar cada um dos comandos a seguir:

- Indexar um documento no índice `workshop`, com ID: 1

```
PUT workshop/_doc/1
{
    "name" : "Introdução ao Elasticsearch",
    "date" : "2019-04-27T13:00:00"
}
```

- Indexar um documento no índice `my_logs`, deixar que o próprio elasticsearch crie o ID

```
PUT my_logs/_doc
{
    "timestamp" : "2019-04-27T13:00:00",
    "application" : "nginx"
}
```

- Forçar que o elasticsearch use a operação `create`, ou seja, se o documento já existe ocorrerá uma exceção

```
PUT workshop/_doc/1/_create
{
    "name" : "Introdução ao Elasticsearch",
    "date" : "2019-04-27T13:00:00"
}
```

- Fazer o get de um documento pelo ID

```
GET workshop/_doc/1

PUT workshop/_doc/1/_update
{
    "doc" : {
        "name" : "Introdução à Elastic Stack"
    }
}
```

- Listar todos os documentos do índice `workshop`

```
GET workshop/_search
```

- Apagar o documento cujo ID = 1

```
DELETE workshop/_doc/1
```

4- Criar um `index pattern` no Kibana e para o índice `my_logs` e abrir a aba `Dicovery` do Kibana

https://www.elastic.co/guide/en/kibana/current/tutorial-define-index.html


