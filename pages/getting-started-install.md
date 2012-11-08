---
title: Instala��o
layout: default
---

## Instala��o via Composer 

Instale o composer no seu projeto:

    curl -s https://getcomposer.org/installer | php

Crie o arquivo `composer.json` na pasta raiz do seu projeto:

    {
        "require": {
            "slim/slim": "2.*"
        }
    }

Instala��o via composer:

    php composer.phar install

Adicione esta linha no seu arquivo `index.php` da aplica��o:

    <?php
    require 'vendor/autoload.php';

## Instala��o Manual

Fa�a o download e extraia os arquivos do Slim Framwork na pasta do seu projeto e fa�a o `require` do Slim no seu 
arquivo `index.php`. Voc� precisar� tamb�m fazer o registro do autoloader do Slim.

    <?php
    require 'Slim/Slim.php';
    \Slim\Slim::registerAutoloader();
