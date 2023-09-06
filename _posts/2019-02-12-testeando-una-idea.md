---
layout: post
author: Daniel Salvat
read_time: true
show_date: true
title:  'Testeando una idea'
date:   2019-02-12 09:32:20 +0200
description: «Tengo una idea brutal para un negocio, pero no voy a contar muchos detalles porque no quiero que me la roben»
img: posts/20190212/idea-1200x279.jpg
tags: [proyectos, servicios, emprender, test]
mathjax: yes
---

«Tengo una idea brutal para un negocio, pero no voy a contar muchos detalles porque no quiero que me la roben»

Creo que todos hemos oído una frase como ésta, o hemos sido nosotros mismos los que la hemos dicho.

La pregunta es ¿cuántos de nosotros ha llevado a cabo esa idea maravillosa que nos iba a convertir en el próximo Bill Gates, o Jeff Bezos del mundo de los negocios?

Y es que emprender, bajo mi óptica, es una aventura fantástica pero requiere de mucha energía, determinación y perseverancia para llevar a cabo aquello que has imaginado. Y lo más importante de todo: mucha valentía. Porque el camino va a ser duro.

Hoy en día, los que nos dedicamos al mundo tecnológico, tenemos ciertas ventajas. Probablemente habrá muchos inconvenientes, como que la competencia puede ser feroz, pero hoy voy a focalizar mi atención en dichas ventajas.

Hasta hace muy pocos años, el tener una idea que requiriera de algún soporte tecnológico, e intentar llevarla a cabo, era muy costoso. Servidores, servicios varios,… todo tenía un coste nada despreciable.

Hoy, con unos euros y probablemente un considerable esfuerzo (la idea maravillosa lo merece, ¿o no?), se puede confirmar o desmentir un nuevo posible negocio tecnológico.

Este mismo enfoque se puede dar en lo que se denomina intraemprendimiento (para saber más del concepto, os invito a visitar uno de los posts de quien acuñó el término, Gifford Pinchot, por si os sentís identificados en alguna de las cuatro categorizaciones que hace).

Aviso que este post no va de emprendimiento. Va del enfoque tecnológico a una posible idea de negocio, y de las percepciones acerca de barreras que ya no son tan altas como antes.

¿QUÉ NECESITO PARA MATERIALIZAR LA IDEA?
Para empezar hay que tener muy claro una cosa: tiene que funcionar, pero no tiene que ser el producto perfecto. Al menos, de momento.

Hay que tener una visión de producto, aunque sin pretensiones de tener el producto finalizado para ponerse en marcha.

Buscamos un MVP, un Producto Viable Mínimo, para arrancar. En estos momentos, no importa si detrás del telón hay alguien moviendo los hilos manualmente. Da igual si no está todo automatizado. El objetivo es saber si a alguien le va a parecer atractivo como para consumirlo en el futuro. Y así justificar el dedicarle más tiempo a desarrollarlo o no.

¿CUÁNTO ME VA A COSTAR TODO?
Aquí es donde quería llegar. Si el producto es tecnológico, una web o una app, vamos a necesitar algunas cosas. Calculemos lo que nos puede costar testear nuestra idea:

El servidor

Un Servidor donde hacer correr mi aplicación y/o donde centralizar la base de datos. Hoy hay muchas plataformas muy interesantes de lo que llamamos VPS (Virtual Private Server, o Servidor Virtual Privado). Yo voy a recomendar aquél que uso: Digital Ocean.

Pongamos que nos damos 3 meses para empezar a poner en marcha el proyecto. Pues bien, el coste de un proyecto pequeño es de entre $5 y $20 al mes. Con lo que el servidor nos va a costar $60 si queremos uno solo (yendo a máximos). Habrá la necesidad de tener otros entornos, pero podemos ser flexibles en cuanto a las dimensiones de los diferentes entorno: $15 para producción y $10 para pruebas, por ejemplo. Total $75 ($25 al mes). Muy asumible.

El dominio y la cuenta de e-mail

También querré un dominio, con un nombre asociado. De la imagen de marca y de todo lo demás, lo dejaría para los profesionales de la comunicación y el diseño. Ellos sabrán mucho mejor qué hacer y cómo.

Como siempre hay varios proveedores de dominio, y aquí no me voy a mojar demasiado. Los hay muy buenos, y a muy buen precio. El precio ronda los 12€ al año.

También querré una cuenta de e-mail. Yo recomiendo Google Suite como herramienta. Por sólo $5 al mes podemos disfrutar del mail, de chat, de calendario, además de una suite interesante de aplicaciones de gestión y, además, ¿quién no tiene una cuenta de Gmail? La curva de aprendizaje es prácticamente nula.

No podemos obviar la seguridad

Con la seguridad en Internet no se puede jugar. Es por ello que hay que asegurarse de hacer nuestra plataforma lo más segura posible.

Para ello es importante contar con una web/app que funcione con protocolo HTTPS. Para ello necesitamos un certificado SSL, el cual podemos obtener de manera totalmente gratuita en la plataforma Let’s encrypt.

En los proyectos en los que he participado, y sin tener un argumento más allá del servicio que ofrecen, he intentado utilizar otros proveedores de SSL comerciales, ya que me facilitan un soporte y unas garantías (por contrato) que considero importante.

Los precios de un certificado SSL hoy en día se mueven por los 15€ al año para proyectos sencillos.

La gestión de los e-mails y las notificaciones

Las campañas de marketing y envíos varios de e-mails son muy importantes, y probablemente sea algo que nos pidan nada más empezar el proyecto.

En mi caso, tengo muy buena experiencia con Sendgrid. Y es que mediante un plan de iniciación, el coste es gratuito para un número envíos de e-mails mensual inferior a 12,000. Y si queremos enviar hasta 40,000 cada mes, el coste es de 15€. Habrá más, pero lo cierto es que estoy muy satisfecho con el servicio hasta el momento.

El Producto

Teniendo todos los servicios y productos externos identificados, me atreviría a decir accesorios, nos queda desarrollar el producto.

El MVP ha sido decidido, con lo que queda decidir con qué tecnologías hay que desarrollarlo.

En mi caso, los criterios principales que utilizo son 2: ¿Con qué tecnologías tiene experiencia el equipo (o yo mismo si el proyecto es personal)? ¿Hay una comunidad fuerte en esta tecnología que me «garantice» que no voy a tener que reescribir el proyecto por falta de soporte en los próximos 3 años, por ejemplo?

¿Dónde guardo el código?

Mantener el código, y sus versiones, accesible para el equipo es muy importante. Para mí hay dos opciones: Bitbucket, cuyo plan gratuito permite repositorios privados para equipos de hasta 5 personas; y Github, que tiene un plan similar (los privados ahora también son gratuitos) pero para hasta 3 personas.

Tanto Bitbucket (soy muy fan de los productos Atlassian – Jira y Confluence los utilizo a diario, además de Trello) como Github me parecen grandes servicios. Cualquiera de los dos es una apuesta segura.

El coste total

Teniendo en cuenta que hemos dicho que testearíamos nuestra idea durante 3 meses, añadimos una previsión (optimista) hasta los 6 meses y eliminando cualquier otro aspecto que no sea puramente las herramientas a usar tenemos:


* El cambio a fecha de hoy (11/02/2019) es 1 Dolar = 0.88 Euros
  ** Suponemos que enviamos más de 40,000 e-mails a partir del mes 4.
  Recuerdo que la intención de este post es destacar herramientas que podemos usar para testear nuestra idea sin arriesgar mucho dinero.

Bonus track

Me dejo muchas herramientas. Algunas no las considero críticas para esta fase, pero es muy interesante conocerlas en el caso en el que deseemos ir más allá: CircleCI (Integración Continua) o Sentry (Tracking de errores) son algunos ejemplos (aunque debo admitir que no tengo mucha experiencia aún con ellos).

¿MI IDEA VALE LA PENA?
Sabiendo ahora que las barreras (de coste) no son tan altas, sólo nos queda preguntarnos si vale la pena ponernos manos a la obra y testear la idea. Las preguntas que suelo hacerme cuando se trata de este tipo de proyectos son:

¿Tiene sentido? ¿Es el mejor proyecto al que nos podemos comprometer ahora mismo? ¿Tenemos el apoyo suficiente?

Son preguntas muy relevantes a la hora de tomar la decisión de continuar por un lado u otro. Tanto si es un proyecto personal como si es uno profesional.

Es posible que le vayamos a dedicar mucho tiempo. Es bueno valorar qué consecuencias puede tener «meterse».

RECAPITULANDO
Definir una Visión de Producto. ¿Cómo queremos que sea nuestro producto final?
Definir un MVP. La mínima expresión de Producto que tenga sentido por sí sola.
Identificar las necesidades tecnológicas y utilizar sólo aquellos recursos que sean imprescindibles, y valorar el coste según lo necesario a corto y medio plazo.
Desarrollar la idea. Ánimo! Creo que es la parte más dificil ya que vamos a necesitar dedicarle tiempo, probablemente el tiempo libre, para poder tener algo funcionando.
Teniendo esta información en la mano, quizás no nos queden excusas para poder llevar a cabo esa idea fantástica. 🙂

Os deseo una feliz semana!