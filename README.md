<div style="background-color: #f5f5f5; padding: 10px; border: 1px solid #ccc; border-radius: 4px; font-family: 'Courier New', monospace;">
  <button onclick="copyCode()" style="background-color: #4CAF50; color: white; padding: 5px 10px; border: none; border-radius: 4px; cursor: pointer;">Seleccionar todo</button>
  <pre><code id="code" style="font-size: 14px;">
// Aquí puedes escribir tu código
  </code></pre>
</div>

<script>
function copyCode() {
  var code = document.getElementById("code");
  var selection = window.getSelection();
  var range = document.createRange();
  range.selectNodeContents(code);
  selection.removeAllRanges();
  selection.addRange(range);
  document.execCommand("copy");
  alert("Código copiado al portapapeles");
}
</script>


Nota: al descargar o clonar el archivo dara un zip y al descompirmirlo dara otro que es donde estaran todos los archivos del proyecto

**Para hacer este proyecto de laravel se utilizo laragon**

  #1 paso descargar laragon <hr>

- Visita la página web oficial de Laragon: https://laragon.org/download/index.html
- descargar esta version: Download Laragon - Full (173 MB)


**# 2 despues de instalo haz los siguentes pasos**<hr>
- Descarga o clona el proyecto desde Github a la carpeta www de Laragon.
- Abre Laragon y asegúrate de que el servidor Apache y MySQL estén activados sino dale en **Iniciar todo** que esta en la **Parte Inferior izquierda**.
- Abre una terminal en la carpeta del proyecto dentro de la carpeta www de Laragon o alli mismo donde dice **Terminal** al lado del **root**.
- Ejecuta el comando 
- <pre><code>
composer install
</code></pre>
**composer install** para instalar las dependencias de Laravel.
- Si el proyecto utiliza algún gestor de paquetes de front-end como npm o Yarn, debes ejecutar el comando **npm install** o **yarn install** para instalar las dependencias de front-end.

**Nota**: puedes ejecutar el proyecto una vez Instaladas las dependencias con el comando **php artisan serve**, si no funciona sigue los pasos: 

#3 migraciones <hr>
- Ejecuta el comando **php artisan migrate** para correr las migraciones de Laravel y crear las tablas necesarias en la base de datos.
- Te pedira crear la tabla dale yes

#4 crear seeders
Ejecuta los siguentes comandos en la terminal para los seeders
-**php artisan db:seed Databaseseeder**

#5 Ver los status de nuestras tablas <
-**php artisan migrate:status**

#6 Hcer los rollback
-**php artisan migrate:rollback**
