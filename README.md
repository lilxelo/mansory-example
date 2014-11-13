Ejemplo de cómo crear un diseño tipo Pinterest con la librería JQuery Mansory
===============

Debido a la flotabilidad de los elementos en CSS, no podemos hacer que elementos de diferente altura se unan, por así decirlo, de forma vertical. Para ello tendremos que usar alguna librería que trabaje en cliente. He eligido la librería Mansory, utilizada de forma muy básica, para crear este efecto.

Mansory dispone de multitud de opciones como podrás ver en su web. http://masonry.desandro.com/

Para recrear un ejemplo básico he creado <div> con fondos de colores diferentes.
Puedes ver el resultado del uso de la librería en el archivo index.html del repo. Observa que es Responsive. 

Para comenzar en el <head> tienes que incluir JQuery y la librería Mansory. 
Posteriormente he escrito en el mismo html el estilo CSS de los diferentes <div>, dándole alturas diferentes a cada uno de ellos. Todos son float:left. 

Finalmente realizamos la llamada a las funciones de la librería Mansory de la siguiente forma: 

$(document).ready(function(){
		var $container = $('#trabajos');
		$container.masonry({
		  columnWidth: 0,
		  itemSelector: '.trabajo'
		});
});


