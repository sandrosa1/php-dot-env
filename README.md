# PHP Variáveis ​​de Ambiente

Uma biblioteca básica para gerenciar variáveis ​​de ambiente em PHP.

## Instrução
Para utilizar ess biblioteca execute o comando abaixo:

```Shell
 $ composer require sandro/php-dot-env
 ```


Depois basta criar um arquivo`.env`na raiz do projeto, nomeando as variaveis sensiveis EX:

```
DB_HOST=localhost
DB_USER=root
DB_PASS=pass
DB_NAME=database
DB_PORT=3306
```

```php
<?php

require __DIR__. '/vendor/autoload.php';

//CARREGAR VARS DO AMBIENTE DO ARQUIVO NA RAIZ

SandroAmancio\DotEnv\Environment::load(__DIR__);

//OBTER VAR DE AMBIENTE
echo getenv('DB_NAME');

```

## Requirementos

PHP >= 7.0
