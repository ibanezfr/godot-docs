# Reglas de estilo para traducir "Godot" al español.

## Introducción

Este documento tiene como objetivo ayudar a unificar el estilo de la traducción
al español de Godot, así como de la documentación de Godot. Se prioriza la 
legibilidad y la claridad.

Para la traducción en sí se utiliza la herramienta [Weblate](https://hosted.weblate.org/projects/godot-engine/)
La [documentación oficial](https://docs.godotengine.org/de/4.x/contributing/documentation/editor_and_docs_localization.html)
proporciona una explicacón más detallada. El funcionamiento de Weblate no se 
aborda en este documento.

Weblate cuenta con un glosario que lista términos frecuentemente utilizados para
asegurar su traducción uniforme. Por lo tanto, en este documento se omite la 
clarificación de la traducción de términos individuales. Si surge alguna 
discrepancia durante la traducción de un término, se debe discutir primero en 
el [chatroom para la traducción de Godot al español](https://chat.godotengine.org/channel/translation-es).

## Recursos técnicos

### Traducciones automáticas y flujo de trabajo

Recomendación principal: evita traducir automaticamente textos que no comprendes, 
una mala traducción solo produce confusión. 

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
* Revisar el texto en busca de desviaciones del glosario y corregirlas si es 
necesario.
* Realizar cambios propios donde sea adecuado.

Además, es recomendable realizar correcciones directamente en el lado derecho de
DeepL, ya que la herramienta puede aprender de correcciones repetidas. Además, 
los términos que se traducen persistentemente de manera incorrecta pueden 
ingresarse en el glosario de DeepL para forzar una traducción específica.

## Reglas de estilo

### Tú o Usted

La traducción actual de Godot utiliza principalmente "tú" en lugar de 
"Usted" en el tratamiento directo. Aunque la forma más amigable de 
"tú" también sería una buena elección en el ámbito de los videojuegos.
Quedan partes de traducciones viejas iniciales que todavía utilizan "Usted", 
estas tienen que figurar como marcadas para edición en weblate y se puede
aprovechar para ajustar a medida se encuentren.

> :arrow_forward: Press the "Add Child Node" button or "Other Node" to create 
> a root node.
>
> :x: Presione el botón "Agregar nodo hijo" u "Otro nodo" para crear
> un nodo raíz.
>
> :heavy_check_mark: Presiona el botón "Agregar nodo hijo" u "Otro nodo" para 
>  crear un nodo raíz.

### Voz pasiva para traducir "we" o "you"
En textos formales en inglés, se suele utilizar "we" o "you" en oraciones como 
las siguientes:

> :arrow_forward: For this purpose, **we** have implemented the following code.
>
> :arrow_forward: This is especially useful when **you** need to export a 
> project.

La traducción literal de estos textos al castellano sería:

> :x: Para este propósito, **hemos** implementado el siguiente código.
>
> :x: Esto es especialmente útil cuando **necesitas** exportar un proyecto.

Sin embargo, el uso de "we" y "you" en casos como los anteriores suele ser una 
forma de voz pasiva. En este sentido, otra traducción posible al castellano 
(utilizando voz pasiva) sería:

> :heavy_check_mark: Para este propósito, **se ha** implementado el siguiente 
> código.
>
> :heavy_check_mark: Esto es especialmente útil cuando **se necesita** exportar
> un proyecto.

Por regla general, "we" y "you" han de traducirse utilizando voz pasiva en el 
contexto de esta documentación. En caso de haber objeción con algún texto en 
particular, se recomienda discutirlo en el chatroom mencionado arriba.


### Principios gramaticales

La traducción de Godot se puede dividir en cuatro bloques generales: *Editor*,
*Propiedades*, *Documentación* y *Referencia de Clases*.


Cada uno de estos bloques tiene requisitos específicos para la traducción. 
Mientras que la documentación están diseñada principalmente para ser 
comprensible y agradable de leer, en el editor y las propiedades a menudo se 
requiere un lenguaje más conciso, ya que a menudo hay espacio limitado para 
los textos.

Por lo tanto, tiene sentido establecer algunas reglas básicas para la 
traducción. Ten en cuenta que estas reglas no son absolutas y, en caso de duda,
se debe traducir con discreción. Sin embargo, tales reglas ayudan a promover un 
estilo de lenguaje uniforme en toda la documentación.

Las siguientes reglas básicas se aplican actualmente en la traducción:

#### Manual/Referencia de Clases


En las *Instrucciones*, se debe mantener la forma gramatical del texto original,
a menos que ello afecte la legibilidad. Generalmente, se debe evitar evitar o 
preferir ciertas construcciones lingüísticas en este punto. A menudo, seguir el 
texto original es la mejor opción. En particular, el uso del tratamiento formal 
"Usted" en esta parte de la documentación es común y debe mantenerse así.

TODO:(buscar ejemplo)
> :arrow_forward: The table of contents in the sidebar should let you easily
> access the documentation for your topic of interest.
>
> :heavy_check_mark: 
> 

<br/>

> :arrow_forward:  To move our icon, we need to update its position and rotation
> every frame in the game loop.
>
> :heavy_check_mark:
> 

<br/>

> :arrow_forward: This build can be manually triggered by clicking the "Build"
> button at the top right of the editor.
>
> :heavy_check_mark: 
> 

En algunas secciones del manual, como ciertos encabezados o enumeraciones, 
se recomienda el [gerundio](https://es.wikipedia.org/wiki/Gerundio) o 
[infinitivo](https://es.wikipedia.org/wiki/Infinitivo):

Ejemplos:
TODO:(buscar ejemplo)
> :arrow_forward: Setting up the project
>
> :heavy_check_mark: 

<br/>

> :arrow_forward: For the player, we need to do the following:
> * Check for input.
> * Move in the given direction.
> * Play the appropriate animation.
>
> :heavy_check_mark: Para el jugador haremos lo siguiente:
> * Comprobar entradas.
> * Moverse en la dirección dada.
> * Reproducir la animación apropiada.

#### Propiedades

Las *Propiedades* son descripciones muy breves de las características de Godot,
que a menudo tienen poco espacio disponible en el editor. Aquí, frecuentemente 
se trata de términos individuales, donde la dificultad radica más en encontrar 
el vocablo correcto (más sobre esto abajo) que en la forma gramatical.

A veces son frases cortas que, en la mayoría de los casos, se traducen mejor al 
infinitivo-imperativo (ver ejemplos arriba), ya que esta forma encaja bien 
lingüísticamente y ocupa poco espacio. Además, aquí se deben omitir los 
artículos cuando sea posible, al igual que suele hacerse en el original.

TODO:(buscar ejemplo)
> :arrow_forward: Keep Screen On
>
> :x:
>
> :heavy_check_mark:

#### Editor

Los textos del *Editor* están compuestos tanto por pequeños bloques de texto, 
por ejemplo, cuando un tooltip describe una configuración en detalle, como por 
términos cortos que a menudo tienen poco espacio disponible.

Al traducir el Editor, se aplican tanto las reglas para las instrucciones como 
las para las propiedades, dependiendo de si el texto a traducir está escrito más
en forma larga o en forma corta.

### No tengas miedo de los términos en inglés

Algunos términos son difíciles de traducir al español. Estos incluyen términos
técnicos que ya se han incorporado al uso del idioma en su forma inglesa
(*Thread*, *Debuggen*, *Spawn-Punkt*).

Otros términos tienen traducciones comunes al español, como *Nodo* para *node*. 
Sin embargo, dado que en el mundo de Godot existen objetos con nombres fijos,
como `Node2D`, también optamos por dejar en inglés las palabras derivadas
de ellos.

TODO:(buscar ejemplo)
> :arrow_forward: We're going to use the ``Input`` singleton here as we need to
> know if the player wants to turn or move every frame.
>
> :x: 
> 
>
> :heavy_check_mark: 
> 


Mientras leas el manual, encontrarás muchos de estos términos que han sido
castellanizados intencionalmente. Esto puede parecer un poco inusual en ciertos
momentos, pero hay muchas situaciones en las que esto ayuda a evitar problemas
de traducción.

Si te encuentras con una regla que parece no tener sentido, es recomendable 
discutirlo en el [Chat](https://chat.godotengine.org/channel/translation-es).
Para tener una visión general de los términos documentados que deben permanecer 
en inglés, es útil echar un vistazo al [Glosario](https://hosted.weblate.org/projects/godot-engine/glossary/es/).
Si un término no está registrado allí, puedes utilizar la función de búsqueda de
Weblate para encontrar ejemplos en las traducciones existentes.

A veces, también es necesario tomar una decisión basada en tu propio criterio o
apartarse de una de las reglas del glosario. Esto está perfectamente bien, ya 
que el lenguaje es complejo y no se puede establecer una solución predefinida 
para cada caso especial.

TODO:(buscar ejemplos)
Ejemplo 1:

> :arrow_forward: Stereo Panning
>
> :x: 
>
> :heavy_check_mark: 

Ejemplo 2:

> :arrow_forward: Drag to pan the view
>
> :x: 
>
> :heavy_check_mark: 


El primer ejemplo proviene del ámbito del audio, donde "Stereo-Panning" es un 
término común. El segundo ejemplo utiliza la palabra "panning" como un término 
general. Aquí no se hace referencia a un lenguaje técnico especializado, por lo 
que la palabra puede ser traducida al alemán de manera normal.

Esta distinción a menudo se refleja en el glosario con dos entradas del mismo 
término. Se proporciona un texto descriptivo para ayudar a explicar en qué 
contexto es apropiada cada traducción.

Más abajo encontrarás consejos de investigación que pueden ayudarte a encontrar 
una traducción adecuada si un término no se encuentra ni en el glosario ni en la
documentación existente.

### Oraciones anidadas

Cuando se traduce directamente una oración en inglés, es fácil caer en la 
tentación de formar oraciones complejas o, en general, muy largas. Aquí es útil
una pretraducción realizada por una IA, que a menudo evita esto bastante bien.
Sin embargo, en general, es simplemente porque las palabras y las oraciones en
castellano tienden a ser más largas que sus equivalentes en inglés.
Por lo tanto, es importante asegurarse de que la traducción al alemán no sea 
demasiado compleja o larga. Puede ser perfectamente válido dividir una oración
en dos, incluso si esto significa que la forma gramatical del original no se
conserva.

TODO:(buscar ejemplo)
> :arrow_forward: Min SDK cannot be lower than %d, which is the version
> needed by the Godot library.
>
> :x: 
> 
>
> :heavy_check_mark: 
> 

<br/>

> :arrow_forward: In addition, one will need a primary GUI for their game that
> manages the various menus and widgets the project needs.
>
> :x: 
> 
>
> :heavy_check_mark: 
> 
>
> :heavy_check_mark: 
> 

### Adiciones propias

Al traducir el manual, asegúrate de traducir solo el texto original, sin hacer 
tus propias adiciones o explicaciones. Si el texto original es incompleto o 
necesita una explicación, solicita primero un cambio en el original o presenta 
tú mismo un Pull-Request en godot-docs. Debemos entender que en Weblate somos 
solo traductores y no autores.

TODO:(buscar ejemplo)
> :arrow_forward:: Computes the arctan of x
>
> :x: 
> 
>
> :heavy_check_mark:
>

## Coherencia entre Editor/Propiedades y Manual

Si cambias un término del Editor o las Propiedades, asegúrate de buscar en la 
página de Weblate del manual esos términos y ajustarlos en consecuencia para 
mantener la coherencia en las traducciones.

También ten en cuenta que un término del Editor o las Propiedades suele aparecer
en varias partes del Editor o las Propiedades, por lo que, siempre que sea 
posible, todas esas instancias deberían traducirse.

## Prueba de la traducción

Para las traducciones del Editor y las Propiedades, es recomendable probarlas 
por uno mismo descargando [la traducción actual](https://docs.godotengine.org/es/4.x/contributing/documentation/editor_and_docs_localization.html#offline-translation-and-testing)
y compilando Godot con los cambios realizados [por uno mismo](https://docs.godotengine.org/es/4.x/contributing/development/compiling/compiling_for_windows.html).

Especialmente en el caso del manual, a menudo es importante considerar el 
contexto entre bloques de texto adyacentes, por lo que leer un artículo completo
puede hacer que se vean errores que podrían pasarse por alto fácilmente 
en Weblate.

## Consejos de investigación

En general, al traducir un término, es importante considerar si se puede 
realizar una traducción correcta basada en la propia experiencia con el idioma,
o si sería mejor investigar un poco más.

La primera fuente para traducir términos establecidos debería ser el glosario y
las traducciones existentes. La función de búsqueda de Weblate es útil en este
sentido.

Si un término no se puede encontrar en estas fuentes o si hay dudas sobre su
corrección, hay algunas otras fuentes útiles:


Conceptos fundamentales científicos:
Puedes buscar términos científicos en la versión en inglés de [Wikipedia](https://www.wikipedia.org).
Desde allí, puedes acceder al artículo en alemán a través del menú de idiomas,
donde a menudo encontrarás una traducción alemana correcta del término.
Sin embargo, asegúrate de que el artículo en alemán describa el mismo
significado que el artículo en inglés.

Términos técnicos generales:
Para otros términos técnicos generales, puedes recurrir a sitios web como
[www.linguee.com](www.linguee.com) para ver cómo han sido traducidos por otros
traductores, a menudo profesionales, en diferentes contextos.

Términos especializados en juegos o diseño de juegos:
Por último, hay términos especializados que provienen directamente de los juegos
o el diseño de juegos. No está de más consultar cómo otros herramientas del
ámbito traducen estos términos (Unity, Unreal). Dado que estas herramientas
cuentan con presupuestos para traductores profesionales, esta es una fuente
especialmente útil para términos muy específicos.

Por último, puede ser útil consultar a desarrolladores experimentados para
aclarar la traducción de un término, ya sea en el [Chat](https://chat.godotengine.org/channel/translation-es)
o en alguno de estos grupos:
- [Godot Engine Hipano](https://discord.com/invite/fp4Z7QmZGu)
- [Godot en español](https://discord.com/invite/2BtycSPdkk)
- [Canal español-general del servidor oficial de Discord](https://discord.gg/4JBkykG)

## Reglas del glosario
Esta sección trata sobre el glosario. Si solo deseas traducir, puedes dejar de 
leer aquí. Sin embargo, si deseas mantener entradas en el glosario, deberías 
seguir leyendo.

El glosario sigue ciertas reglas que deben tenerse en cuenta:

### ¿Qué se incluye en el glosario?
El glosario es útil cuando se quiere traducir una palabra de manera consistente
en diferentes partes del texto. Siempre que se desee garantizar esto, también 
es útil tener una entrada en el glosario. Sin embargo, también hay que tener en
cuenta que un glosario muy grande requiere mucho trabajo de mantenimiento.
Por lo tanto, no es necesario que cada palabra tenga una entrada en el glosario.

TODO:(buscar ejemplos)
> :x: color -> color

La palabra "color" es bastante clara y probablemente no necesite una explicación
explícita en un glosario.


> :heavy_check_mark: Buffering -> Buffering

Aquí, el glosario indica que el término es un término técnico establecido que no
tiene una buena traducción al español y, por lo tanto, se mantiene en inglés.

### Una palabra, múltiples significados
Si una palabra en inglés puede ser traducida de varias maneras, entonces se debería crear una entrada separada en el glosario para cada traducción. Esto ayuda a la legibilidad y facilita agregar más significados más adelante.

TODO: (Buscar un buen ejemplo)
> :x: volume -> Volumen, Lautstärke
>
> :heavy_check_mark: volume -> Volumen (*Translation Explanation:* im Sinne von &bdquo;Rauminhalt&rdquo;)
>
> :heavy_check_mark: volume -> Lautstärke (*Translation Explanation:* im Audio-Kontext)

Es recomendable utilizar el campo de "Translation Explanation:" para describir
cómo difieren las diferentes traducciones y en qué casos se deben usar.

**Atención**: Existe también el campo de "Explanation" destinado a explicar el
texto original. Este campo no debería ser utilizado, ya que puede causar
entradas duplicadas no deseadas en la barra lateral.


### Utilizar formas básicas

Un palabra en inglés debería ser ingresada en el glosario en su forma más básica
para que pueda ser automáticamente asignada en la mayor cantidad de casos
posible. Esto significa que los verbos deberían estar en su forma base
(**importante**: sin *to*) y los sustantivos en singular.

Ejemplos:

> :x: to hide -> ocultar
>
> :heavy_check_mark: hide -> ocultar

<br/>

> :x: constants -> constantes
>
> :heavy_check_mark: constant -> constante

Lamentablemente, la versión actual de Weblate no admite variantes morfológicas.
Por lo tanto, si una palabra en el glosario se indica en singular, solo se
ofrecerá durante la traducción si también se usa el singular en el texto de
traducción. Ya existe un [ticket](https://github.com/WeblateOrg/weblate/issues/3023)
sobre este problema en el repositorio de GitHub de Weblate. Hasta que se
resuelva este problema, debemos evitar como solución temporal crear entradas en
el glosario tanto en singular como en plural, ya que esto dificulta su
mantenimiento.

### Terminology
Una entrada marcada como "Terminology" se incluirá automáticamente en todos los
demás idiomas en los glosarios y generará tareas pendientes abiertas allí.

Esto puede resultar en la aparición de nuevas entradas en el glosario en la
traducción al español, porque otro idioma las ha añadido. En este caso, es
válido quitar la marca de Terminology y eliminar la entrada si consideramos que
no tiene sentido. Este proceso no alterará la entrada en ningún otro idioma.

En principio, no deberíamos marcar la entrada con la flag de Terminology, ya que
potencialmente podría saturar los glosarios de otros idiomas, especialmente si
tienen diferentes criterios para determinar qué tipos de términos califican
como "Terminology".

### Untranslatable

Una entrada marcada como "untranslatable" es un término que deliberadamente no
se debe traducir, como términos establecidos como `Android` o `OpenGL`. Sin
embargo, muchos de estos términos realmente no tienen lugar en el glosario, por
lo que esta etiqueta no debería usarse con demasiada frecuencia.
Puedes identificar un término marcado como "untranslatable" porque aparece
resaltado en amarillo cuando se muestra en la barra lateral del glosario.

### Forbidden Translation
Una entrada marcada como "Forbidden translation" se puede utilizar para mostrar
una traducción que no debe ser utilizada, por ejemplo, porque representa un
[Falso amigo](https://es.wikipedia.org/wiki/Falso_amigo) propenso a errores, o
para bloquear ciertos términos en castellano.
TODO: (Buscar buen ejemplo)
Por ejemplo, podríamos acordar
traducir consistentemente el término privacy como privacidad y no como el más técnico
intimidad. En ese caso, ambos términos se agregarían al glosario, pero el segundo se
marcaría como "Forbidden translation".

## Cambios en este documento
Cualquier cambio en este documento debe ser discutido en el [Chat](https://chat.godotengine.org/channel/translation-es) y, una vez resuelto, se debe realizar un Pull Request para committear los cambios en el repositorio de Github.

Nota: Esta guía aún no será subida al repo oficial, debemos dejarla bien para una primera versión.
