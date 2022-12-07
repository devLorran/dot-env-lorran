**# 1 - VARIÁVEIS PARA CONFIGURAR A CONEXÃO COM O BANCO DE DADOS NO ARQUIVO .env QUE FICA NA RAIZ DO PROEJTO #**
    DB_HOST=localhost
    DB_USER=root
    DB_PASS=pass
    DB_NAME=database
    DB_PORT=3306
**# 2 - CARREGA O ENVIRONMENT #**
    <?php

    require 'vendor/autoload.php';

    //LOAD ENVIRONMENT VARS FROM FILE ON ROOT
    LorranCode\DotEnv\Environment::load(__DIR__);

    //GET ENVIRONMENT VAR
    echo getenv('DB_HOST');