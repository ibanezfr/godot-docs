# Las reglas de estilo para traducir "Godot" al español.

## Introducción

Este documento tiene como objetivo ayudar a unificar el estilo de la traducción
al español de Godot, así como de la documentación de Godot. Se prioriza la 
legibilidad y la claridad.

Para la traducción en sí se utiliza la herramienta [Weblate](https://hosted.weblate.org/projects/godot-engine/)
La [documentación oficial](https://docs.godotengine.org/de/4.x/contributing/documentation/editor_and_docs_localization.html) proporciona una explicacón más detallada. El funcionamiento de Weblate no se aborda en este documento.

Weblate cuenta con un glosario que lista términos frecuentemente utilizados para
asegurar su traducción uniforme. Por lo tanto, en este documento se omite la 
clarificación de la traducción de términos individuales. Si surge alguna 
discrepancia durante la traducción de un término, se debe discutir primero en 
el [chatroom para la traducción de Godot al español](https://chat.godotengine.org/channel/translation-es).

## Recursos técnicos

### Traducciones automáticas y flujo de trabajo

La experiencia muestra que la traducción de textos más largos, por ejemplo, de 
las instrucciones o la referencia de clases, a menudo conduce a resultados más 
rápidos y mejores cuando se permite que una inteligencia artificial traduzca el
texto original de antemano.

Un servicio de traducción muy recomendable es el sitio web 
https://www.deepl.com, que proporciona excelentes traducciones iniciales y, en 
muchos casos, conserva correctamente los caracteres de formato, como negritas o 
enlaces, en la traducción.

Otra ventaja de este método de traducción es que es muy probable que un mismo 
texto se traduzca estructuralmente de manera similar en repetidas ocasiones, lo 
cual puede ser muy útil cuando los textos originales cambian ligeramente y la 
traducción pregenerada sigue estando muy cerca de la traducción anterior.

Aquí hay un flujo de trabajo recomendado para la traducción de un bloque de 
texto:

* Copiar el texto original.
* Traducirlo en DeepL.
* Pegar la traducción en el campo de traducción.
* Revisar el texto en busca de desviaciones del glosario y corregirlas si es necesario.
* Realizar cambios propios donde sea adecuado.

Además, es recomendable realizar correcciones directamente en el lado derecho de
DeepL, ya que la herramienta puede aprender de correcciones repetidas. Además, 
los términos que se traducen persistentemente de manera incorrecta pueden 
ingresarse en el glosario de DeepL para forzar una traducción específica.

## Reglas de estilo

### Tú o Usted

La traducción actual de Godot utiliza &bdquo;usted&rdquo; en lugar de 
&bdquo;tú&rdquo; en el tratamiento directo. Aunque la forma más amigable de 
&bdquo;tú&rdquo; también sería una buena elección en el ámbito de los 
videojuegos, cambiarla requeriría mucho trabajo. La discusión sobre cambiar a 
&bdquo;tú&rdquo; depende principalmente de si se puede encontrar 
una cantidad suficientemente grande de voluntarios para cambiar toda la 
documentación. Hasta entonces, por razones prácticas, la traducción debería 
permanecer en la forma más formal de &bdquo;usted&rdquo;.

> :arrow_forward: You can also use the search function in the top-left corner.
>
> :x: También puedes usar la función de búsqueda en la esquina superior izquierda.
>
> :heavy_check_mark: También puede utilizar la función de búsqueda en la esquina superior izquierda.


