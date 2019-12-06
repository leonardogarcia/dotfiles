# Docker Development

### Serviços disponiveis:
- Nginx
- PHP 5.6
- MySQL
- RabbitMQ
- MongoDB
- Redis

### Getting Started

para construir todo o ambiente de desenvolvimento é muito simples:

1. Adicione na raiz do projeto a pasta **dump** com o arquivo **(db_raia.sql)**
    
    Obs..: no repositorio do projeto, na aba Downloads, é possivel baixar o dump.
    
    ```sh
        dump/rd_raia.sql
    ```
2. Agora execute o seguite comando e aguarde a instalação:

    ```sh
        sudo bin/setup
    ```

Ao final da execução, reinicie o seu navegador.
   
#### Utilities

- Docker

    ```
        # iniciar container
        bin/webdev start  

        # stop containers
        bin/webdev stop
        
        # restart containers
        bin/webdev restart
  
        # ver status containers
        bin/webdev status
  
    ```
- PHP

    ```
        # access php bash
        bin/php
  
        # run script php in container
        bin/php [arg]   
    ```

- Mysql 

    ```
        host: 127.0.0.1   
        user: usr_drogasil
        pass: 123123
        
        /** user root */
        user: root
        pass: 123123
    ```
  
- Clean Full Cache 

    ```
        bin/cache
    ```  

- Redis  

    Para acessar o console do redis:

    ```
        bin/redis
    ``` 
    
    Limpar o cache do redis
    
    ```
        bin/redis clean
    ```  
  
 - Magerun
 
     Limpar o cache do magento
     
    ```
        bin/magenrun cache:clean;
   
        bin/magenrun cache:flush;
   
        //or
   
        bin/magenrun cache:clean; bin/magenrun cache:flush; 
    ``` 
    para ver a lista de funcionalidades do Magerun
    
    ```
        bin/magenrun
    ```      

- SSL 

    ```
        # enable cert
        bin/ssl
    ```       
