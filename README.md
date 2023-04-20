Rama a calificar

# # 1 Descargar Laragon<hr>

- Visita la página de Laragon: https://laragon.org/download/index.html y descargar la version: **Download Laragon - Full (173 MB)**


# # 2 despues de instalo hacer los siguentes pasos<hr>
- Descarga o clona el proyecto desde Github a la carpeta www de Laragon.
- Asegúrate de que el servidor Apache y MySQL estén activados en Laragon.
- Abre una terminal en la carpeta del proyecto dentro de la carpeta www de Laragon.
- Ejecuta el comando "composer install" para instalar las dependencias de Laravel

  - <pre><code> composer install</code></pre>
  
- instalar las dependencias de front-end

  - <pre><code> npm install </code></pre>

# # 3 Migraciones <hr>
- Ejecuta el comando para correr las migraciones de Laravel y crear las tablas necesarias en la base de datos

 - <pre><code> php artisan migrate</code></pre>
 
- Te pedira crear la tabla dale yes

# #4 crear seeders<hr>
- Ejecuta los siguentes comandos en la terminal para los seeders
<pre><code> php artisan db:seed Databaseseeder</code></pre>

# # 5 Ver los status de nuestras tablas <hr>
<pre><code> php artisan migrate:statu</code></pre>

# # 6 Hacer los rollback<hr>
<pre><code>php artisan migrate:rollback</code></pre>

# # 7 Postman Consumir servicios<hr>
- descarga el drive y importalo en postman para tener las collecciones
https://drive.google.com/file/d/1ab9mx-BbazYzok3CMHiMO9owwzsVFOGR/view?usp=share_lin
