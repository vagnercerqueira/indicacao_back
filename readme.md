O FRONT END DO PROJETO FOI FEITO EM ANGULAR CLI

API PROJETO UTILIZANDO O FRAMEWORK PHP LARAVEL, NA VERSAO : 8.83.5

BANCO DE DADOS POSTGRES: 10.20.1

PHP VERSAO: 7.4.28

ALTERAR O ARQUIVO:

.env  para configurar os dados de usuario do banco de dados



app->config->database.php

            'pgsql' => [
            
            'driver' => 'pgsql',
            
            'url' => env('DATABASE_URL'),
            
            'host' => env('DB_HOST', '127.0.0.1'),
            
            'port' => env('DB_PORT', '5432'),
            
            'database' => env('DB_DATABASE', 'forge'),
            
            'username' => env('DB_USERNAME', 'forge'),
            
            'password' => env('DB_PASSWORD', ''),
            
            'charset' => 'utf8',
            
            'prefix' => '',
            
            'prefix_indexes' => true,
            
            'schema' => 'indicacao',
            
            'sslmode' => 'prefer',
        ],
        
CRIAR A BASE DE DADOS indicacao

RODAR OS SEGUINTES COMANDOS COM O COMPOSER:

    php artisan migrate   --ira criar as tabelas necessarias para o projeto
    
    php artisan serve      -- ira executar o servidor para rodar o projeto laravel
