# Instalar o APM

- Abra as instruções de instalação diretamente no [Kibana](http://localhost:5601/app/kibana#/home/tutorial/apm).

- Siga as instruções do seu sistema operacional

- Faça o download do arquivo `index.js` e salve em uma pasta:

    $ wget https://raw.githubusercontent.com/tamros/elastic_stack_workshop/master/index.js

- Siga as instruções no Kibana para instalar o agente NodeJS

- Inicie o servidor: 

    ```
    $npm init
    $npm install express --save
    $node index.js
    ```

* Acesse a página principal:
    
    http://localhost:3000/	

* Explore os dados do APM dentro do Kibana
