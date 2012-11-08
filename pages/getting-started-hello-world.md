---
title: Olá Mundo
layout: default
---

Instancie o Slim Framework:

    $app = new \Slim\Slim();

Defina uma rota do tipo HTTP GET:

    $app->get('/hello/:name', function ($name) {
        echo "Hello, $name";
    });

Execute a aplicação:

    $app->run();
