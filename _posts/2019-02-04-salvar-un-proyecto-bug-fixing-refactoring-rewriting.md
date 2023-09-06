---
layout: post
author: Daniel Salvat
read_time: true
show_date: true
title:  'Salvar un proyecto: Bug fixing, refactoring, rewriting'
date:   2019-02-04 09:32:20 +0200
description: Es difícil no caer inmediatamente en la tentación de visualizar cómo sería el mismo proyecto, usando «una tecnología como tiene que ser, y no la que tenemos ahora, que es un dolor de cabeza«.
img: posts/20190204/Salvar-un-proyecto-1200x295.jpg
tags: [proyectos, bug fixing, tecnologia, cto]
mathjax: yes
---

Hace unos años, cuando aún jugaba a baloncesto y me encontraba ya alrededor de los treinta, solía repetir una frase que indicaba claramente que ya estaba dando los últimos coletazos.

«Me encantaría volver a tener veinte años, pero sabiendo lo que sé ahora»

Y es que, metáforas deportivas aparte, uno mira hacia atrás y probablemente habrá una serie de decisiones que hubiera tomado de distinta manera de saber qué consecuencias futuras le esperaban.

Es obvio que uno toma las mejores decisiones basándose en la información que tiene en el momento en el que la tiene. Con lo que mirar al pasado, con la idea de lo que se pudo hacer y no se hizo, no tiene ningún sentido. Y, sin embargo, lo hacemos (al menos yo!).

EL DILEMA
Eso mismo pasa, a mi entender, con un proyecto de software. Pasados unos años, después de haber lanzado con cierto éxito un producto, y haberlo hecho evolucionar, siempre llega el momento en el que se plantean varias opciones:

¿hay que seguir dando soporte, mediante bug fixing, y evolutivos? ¿debemos detectar aquellas partes del código en las que podamos mejorar la eficiencia, tanto a nivel de rendimiento como a nivel de arquitectura, para hacerlo más manejable? ¿o ya no queda otra opción que la de reescribir todo el proyecto?

Cuando se tiene esta conversación, se detectan rápidamente las diferentes posturas:

LA PERSPECTIVA DEL EQUIPO DE DESARROLLO
El equipo de desarrollo, quien se «pelea» con el producto cada vez que tiene que añadirle alguna funcionalidad más o arreglar algún error (también conocido como bug), interpreta esta situación como la oportunidad de manifestar su frustración por tener que lidiar con semejante carga.

La cantidad de nuevos frameworks de desarrollo, que hacen el trabajo mucho más eficiente que los tradicionales, hacen efecto llamada para cualquiera que quiera estar al día.

Blogs y plataformas muy conocidas hacen análisis de qué frameworks son los mejores para trabajar, como la plataforma de Medium, a la que estoy suscrito y recomiendo totalmente, en los que te dicen cómo hacer el CodingTheSmartWay, o las listas de frameworks en HakerNoon (también muy interesante) para el 2019.

Es difícil no caer inmediatamente en la tentación de visualizar cómo sería el mismo proyecto, usando «una tecnología como tiene que ser, y no la que tenemos ahora, que es un dolor de cabeza«.

LA PERSPECTIVA DEL RESPONSABLE DEL EQUIPO
De igual modo que existe la postura del «hay que hacerlo por el bien del proyecto», personificada en el equipo de desarrollo, existe la postura del conservador. Ésta suele ser representada por el responsable del departamento, el CTO, o el nombre que le haya dado la empresa a quien toma las decisiones acerca de a qué proyectos hay que darles foco.

Generalmente, el CTO es reacio a reescribir un producto, por el simple hecho de que requiere un esfuerzo muy grande para estar en el mismo sitio, y no ofrecer un valor añadido palpable (¿os suena el concepto de Coste de Oportunidad?)

Existe otros factores a tener en cuenta. Como por ejemplo que, a priori, no existe ninguna garantía de que una reescritura del producto vaya a solucionar el problema al que ya se está enfrentando el departamento.

Si en su momento se tomó una serie de decisiones a nivel de tecnología, y ha resultado no ser 100% sostenible, ¿qué nos hace pensar que la siguiente decisión vaya a serlo? ¿nos encontraremos con el mismo dilema dentro de un tiempo? ¿Los frameworks de moda hoy, seguirán siendo soportados en los próximos años?

LOS CRITERIOS
Entendiendo que el factor emocional, frustración por un lado e incertidumbre por el otro, no debe ser obviado en ningún caso tenemos la ocasión de aplicarle cierta lógica al asunto, por parte de ambas posturas.

El objetivo (purpose) del producto

Destaco una obviedad, pero no por ello debo dejar de mencionarlo: un producto que no cumple con su objetivo debe ser replanteado de inmediato.

Es el motivo más fuerte por el que hay que reescribirlo. Entrará en desuso de un momento a otro. Es muy importante recabar las métricas adecuadas para saber si eso ya ha pasado o no.

El factor de deuda técnica (Technical Debt)

La definición que podemos encontrar en la Wikipedia es el coste en tiempo de reescribir, esta vez correctamente, una porción de código que no es eficiente o correcta, y que puede acarrear consecuencias en el futuro de la aplicación.

Bajo mi punto de vista, es importante hacer una lectura objectiva de cuánto estamos hablando.

Uno de los muchos artículos que hay por Internet acerca del tema, hace referencia a precisamente eso: What Technical Debt Is and How to Calculate It.

Así que la recomendación es poner el código bajo análisis, usando herramientas como SonarQube, y ver qué lectura hace de nuestro proyecto.

Dicha herramienta utiliza la metodología SQALE (Software Quality Assessment based on Lifecycle Expectations) para elaborar un ratio de estimación de coste de arreglar el código defectuoso, en comparación a reescribir el proyecto entero. (más info aquí).

Conocer, en números, cuál es nuestra deuda técnica es un criterio fuerte a la hora de tomar la decisión de rehacer un producto.

La arquitectura

Hoy en día se puede cambiar un producto software web, sin necesidad de prescindir de todo el software desarrollado.

A la ya conocidísima arquitectura MVC, se añade las MVP y MVVM, aunque MVC siempre ha sido la más popular. Y luego tenemos la  opción de REST APIs, para una arquitectura de BackEnd y FrontEnd, y los micro servicios… un sinfín de posibilidades.

Aunque el impulso sea el de «tirarlo todo a la basura y empezar de nuevo», es importante valorar la posibilidad de mantener cierto core de la aplicación, y decidir qué parte es la que se puede reescribir, refactorizar o, simplemente, actualizar.

El TCO (Total Cost of Ownership)

Sabemos que el TCO de un producto es el coste desde que escribimos la primera linea de código, hasta que desmantelamos la aplicación, o la sustituímos.

Siendo muy poco estrictos, y teniendo en cuenta que lo que se plantea aquí es sustituir el producto por otro con la misma necesidad de recursos (Servidores, red, electricidad… ), el factor diferencial es el coste operativo relacionado con la estabilidad (si ese puede ser un factor), y los costes futuros de evolutivos y actualizaciones.

Bajo mi punto de vista, diferenciar entre el producto actual y la «promesa» del producto futuro, es una mera adivinación. Hay tantos factores que no están bajo nuestro control, que nos es imposible predecir si estamos tomando la mejor decisión bajo este criterio o no.

La expertise del equipo de desarrollo

Un factor clave. Si el equipo de desarrollo desconoce la tecnología que hay detrás de un producto, hay que ponerle remedio.

La primera opción es incorporar, si eso es posible, a alguien con el conocimiento adecuado en dicha tecnología.

De no ser posible incorporarlo, hay que formar a alguien del equipo para que adquiera ese conocimiento. Y si es más de uno, mejor. Y aquí interviene el factor motivacional.

La motivación del equipo

¿A quién le interesa aprender una tecnología que no está de moda? ¿O que es difícil de aprender? ¿Quién quiere invertir tiempo en una habilidad que no es buscada en el mercado?

Es imposible no tener en cuenta este aspecto en la toma de decisiones. Pero también es necesario saber que éste no debe ser el aspecto que haga decantar la balanza hacia una reescritura del producto.

CONCLUSIONES
Como en el 99,9% de los casos, no hay negros ni blancos. Hay toda una gama de grises a tener en cuenta.

No únicamente por factores económicos vamos a dejar de obviar un mensaje que nos está llegando del equipo de desarrollo. Probablemente tengan un criterio tecnológico acertado a la hora de plantear el problema.

Pero tampoco debemos dejarnos llevar por factores emocionales, de frustración.

Dentro de esa extensa gama de grises, habrá soluciones que puedan satisfacer todos los criterios. Probablemente no lo hará al 100% en todos los casos, pero se acercará.

Monitorizar la deuda técnica; separar las diferentes capas de la arquitectura; ofrecer alternativas que permitan modernizar el producto sin necesidad de tener que renovarlo todo… son alternativas a tener muy en cuenta. Hay que ser creativos a la hora de plantear una solución.

Es un reto bonito al que se enfrentan tanto el equipo de desarrollo como su responsable.

¡Ánimo en la búsqueda de grises!

Feliz semana!