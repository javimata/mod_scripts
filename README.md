# mod_scripts

Simple modulo para agregar un Script o codigo en cualquier posición que le indiquemos

Normalmente se puede asignar modulo a la posición Debug o alguna otra que no sea visible normalmente.

## Contenido
Este modulo incluye simplemente 2 archivos:

El archivo mod_scripts.xml es el archivo manifiesto del modulo.
El mod_scripts.php que es el archivo que muestra el codigo ingresado en la configuración del modulo.

### Consejo
Agrega el modulo a una posición ya sea asignada en el header o oculta tipo la posición debug

En el campo de texto de la configuración podrás agregar el script a agregar.

Asegurate de seleccionar Mostrar titulo como Ocultar y de ser necesario en Avanzado selecciona en Estilo de modulo como "none" para dejar lo más limpio posible el modulo.

Si requieres agregar jQuery por ejemplo te recomiendo agregar algo así:

```
(function($){

	$(document).ready(function () {
  
    // Tu codigo jQuery AQUI
  
	});

})(jQuery);
```
