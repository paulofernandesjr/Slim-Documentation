---
title: Instalação
layout: default
---

## Instalação via Composer 

Instale o composer no seu projeto:

    curl -s https://getcomposer.org/installer | php

Crie o arquivo `composer.json` na pasta raiz do seu projeto:

    {
        "require": {
            "slim/slim": "2.*"
        }
    }

Instalação via composer:

    php composer.phar install

Adicione esta linha no seu arquivo `index.php` da aplicação:

    <?php
    require 'vendor/autoload.php';

## Instalação Manual

Faça o download e extraia os arquivos do Slim Framwork na pasta do seu projeto e faça o `require` do Slim no seu 
arquivo `index.php`. Você precisará também fazer o registro do autoloader do Slim.

    <?php
    require 'Slim/Slim.php';
    \Slim\Slim::registerAutoloader();
