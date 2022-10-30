### INSTALACION Y CONFIG


                                                                                                                         
        
 ██████   ██     
██  ████ ███     
██ ██ ██  ██     
████  ██  ██     
 ██████   ██     
                 
                 


### PRIMEROS PASOS PARA INTACLACION Y CONFIGURACION DE LARAVE BY COMPOSER


###  Intslalacion ubicada en el directorio de Xampp *Htdocs* el directorio odnde corre pordefecto xampp para corre proyecto de forma local

 [C://Xampp/htdocs]


### Install laravel composer global

	composer global require laravl/installer


### Descarga de proyecto by Composer x laravel y asiganacion de el  nombre del proyeto  

	composer craete-proyect --prefer-dist laravel/laravel test


## Corre por servidor artisan el proyecto con artisan serv

	[cd test]
	[php artisan serve]



## Instalacion de front end by *Raect Js* por medio de php breeze

# Descarga del proyecto React Js con Breeze

composer require laravel/breeze --dev

# Instala el proyecto descragado 

	php artisan breeze:install react


#### *[Configuracion de el nombre de la base de datos]*  ###  



*/* Asiganr un nombre ala base de d datos y configurar los puertos de tu xampp y directorio de phpmyadmin */*

[Directorio Vizual code ](Archivos ubicados debajo de la carpeta  *VEDOR*)      
    {
        /.env
        /.env.example
    }
            {
                
                DB_CONNECTION=mysql 
                DB_HOST=127.0.0.1
                DB_PORT=3306
                DB_DATABASE= *[NOMBRE DE LA BASE DE DATOS QUE PONDRAS]*
                DB_USERNAME=  *[EN CASO DDE TENER USUARIO Y CONTRASEÑA PONERLOS ]*
                DB_PASSWORD=
            }

# correlo por medio de el servidor de php 

	php artisan migrate


# Migrar la base de datos y configurar para ostart en el servidor de php

*[Preparacion del proyecto ,configuracion y instalarcion del el proyexto para mostrar de manera local]*

*    npm install && npm run dev

    php artisan migrate  
    
    Puedes observar el sitio web desde el servidor con la direccion siguiente
            >  http://localhost:8000.
*

# ------------------01 FINISH COMPLETE LOGIN---------------

- [ ] https://github.com/octo-org/octo-repo/issues/*01 COMPLETADO*740
- [ ] - [x] 02  LARAVEL MVC #7394
- [ ] - [x] 03               #739

> 01 CHEK ACOMPLETADO
     01 Instalacion configuracion laravel bootcamp Mysql react login Register Dashboard


     - [x] #01 Completado / Enelace documentacion official laravel Bootcamp ::- [x] #739



# ------------------02 LARAVEL REACT BD MVC---------------

>02  Models, migrations, and controllers *[SIGUIENTE]*
    You're now ready to start building your new application! Let's allow our users to post short messages called Chirps.


### Instalarcion del la estrctura MVC
*/*
Models provide a powerful and enjoyable interface for you to interact with the tables in your database.

Migrations allow you to easily create and modify the tables in your database. They ensure that the same database structure exists everywhere that your application runs.

Controllers are responsible for processing requests made to your application and returning a response.
*/*


>php artisan make:model -mrc Chirp

### ROUTA/WEB.PHP

>routes/web.php
    Archvio php

<?php
 
use App\Http\Controllers\ChirpController;
use Illuminate\Foundation\Application;
use Illuminate\Support\Facades\Route;
use Inertia\Inertia;
 ...
Route::get('/dashboard', function () {
    return Inertia::render('Dashboard');
})->middleware(['auth', 'verified'])->name('dashboard');
 
Route::resource('chirps', ChirpController::class)
    ->only(['index', 'store'])
    ->middleware(['auth', 'verified']);
 
require __DIR__.'/auth.php';





## CODE EJEMPLO
console.log('Code Tab A');

console.log('a code block');

```javascript I'm A tab
console.log('Code Tab A');
```

```javascript I'm tab B
console.log('Code Tab B');

.markdown-body {
  --md-code-background: #e3dcef;
  --md-code-text: #4a2b7b;
  --md-code-tabs: #c6b8dd;
  --md-code-radius: 4px;
}


```