---
title: "Debian Lo Bueno"
date: 2024-09-05T21:05:06+02:00
author: "emilio.red"
description: "Mi opinión sobre el uso de Debian y sus características."
draft: false
---

Hola a todos, hoy comentaré mis pensamientos y opiniones sobre el sistema operativo Debian.

# Debian

Debian es un sistema operativo GNU/Linux que destaca su increible estabilidad, seguridad y rendimiento. Tanto es así que muchísimas distribuciones de Linux se basan en él. Debido a lo largo que es el artículo lo dividiré en tres partes.

## Lo bueno

Como he comentado es increiblemente estable, esto te permite tener la seguridad que el sistema operativo sólamente va ha petar por tu culpa. jajaja, Me explico:

### La carente inestabilidad en Debian

Definimos inestabilidad a esos momentos donde el Sistema Operativo no se comporta de forma determinista o como deseamos.
Pues bien, ¿Cuándo ocurre? Ocurre cuando lo configuras mal (el SO), es decir, la inestabilidad la proporciona el usuario, no los programas, las librerías, o alguna mala configuración de base. 
Entonces podemos concluir que es el propio usuario quien hace que el sistema operativo sea inestable, eso es algo bueno, porque a diferencia de otros sistemas operativos como Arch, EndeavourOS o Windows (por decir algunos), si tienes algún problema de inestabilidad, es simplemente por una mala configuración, que ha hecho que sea inestable.
Por lo tanto, Debian es uno de los sistemas operativos más estables actualmente en Linux. Y ese hecho personalmente me encanta. Si le tengo que sacar algo malo a eso (que es rizar el rizo), es que a diferencia de otros SO como Arch, en Debian cuando lo configuras todo ya lo tienes para siempre, es decir, es más "aburrido" porque no estás continuamente trasteando y probando nuevas configuraciones, lo cual según como se mire puede ser algo bueno (para los que no se quieren complicar la vida con errores absurdos, como instalar una actualización y que esta provoque errores) o algo malo para la gente que quiere estar continuamente tocando cosas y configuraciones en Linux.
La gracia de esta estabilidad, es configurarlo todo y olvidarte. Tener la seguridad de que tu SO se va a comportar igual ahora que dentro de 5 años incluso actualizándolo regularmente, eso con otros SO no pasa, como en Windows o Arch por ejemplo que puedes actualizarlo y que te salga un Kernel Panic.

### Jugabilidad en Linux

Este apartado no se aplica solamente a Debian, tengo entendido que ocurre en otras distribuciones GNU/Linux, como Arch por ejemplo; pero lo que comentaré será sólamente aplicado a Debian.
Es indudable que hace unos años, la jugabilidad o el "gaming" en linux era una mierda. Sólamente podías jugar juegos compilados y adaptados específicamente para Linux, eso sólamente lo hacían algunas empresas grandes (como Valve con sus juegos), y ni siquiera esas pocas empresas adaptaban todos sus juegos, sólamente algunos. Entonces, cuando querías jugar a un juego, era una ruleta rusa, si tenías suerte funcionaba, y si tenías más suerte aún era sólamente descargar y jugar (cosa que era prácticamente imposible). Eso hacía que muchas veces no querías jugar diréctamente por la pesadez de esa configuración. Eso con los años a cambiado radicalmente para bien, gracias a Proton.

#### Proton

Proton es la capa de traducción de instrucciones de Windows a Linux, está construido sobre Wine, y se encarga de que cuando ejecutas el juego, traduce las instrucciones DirectX, Vulcan, OpenGL (que son librerías Gráficas) y las instruciones nativas de librerías Windows (aka DDLs) a instrucciones que pueda interpretar Linux.
Pues bien, a pesar de que en teoría, este hecho debería ser inestable, en muchos juegos no debería funcionar o joderte la experiencia a mitad de juego. Nada más lejos de la realidad, en la práctica, Proton es sorprendentemente estable, con muy muy muy buen rendimiento donde la mayoría de veces (basado en mi experiencia) los FPS son mejores que diréctamente ejecutar el juego en Windows. Prácticamente nunca aparecen Gliches gráficos o el juego se vuelve inestable. También hay que destacar que aparte de todas estas ventajas, también tiene un foro [ProtonDB](protondb.com) donde hay una comunidad que cuenta las configuraciones que han utilizado para conseguir tener una experiencia aceptable.

Podemos concluir que Valve junto con Steam y Proton, han conseguido renacer el "gaming" en Linux al hacer que la experiencia sea como debería ser, DESCARGAR Y JUGAR.

### Privacidad y Comunidad de Código Abierto

#### Comunidad de Código Abierto

Por defecto Debian sólamente te permite tener los repositorios de Código Abierto, aunque eso puede ser algo malo (lo explicaré en los siguientes apartados) puedes cambiar la configuración de los repositorios fácilmente.
Da bastante seguridad saber que por detras, siempre se prioriza el Código Abierto, debido a que Debian no te hará cosas raras como ocurre en Ubuntu, que de repente te mete programas propietarios o te mete una promoción de Amazon instalándote Bloatware (esto es real, lo empezó a hacer Ubuntu para recaudar más fondos hace años).
Para concluir y no extenderme más, veo como algo bueno que siempre se priorice el Código Abierto por parte de una distribución, y que el sistema operativo sea gestionado por la comunidad y no por alguna empresa por detras.

#### Privacidad

Debido al apartado anterior, los desarrolladores de Debian no tienen ningún motivo para obtener ninguno de tus datos, al no haber ningún incentivo monetario, como ocurre con Windows o Ubuntu, tienes la seguridad que a los desarrolladores de Debian nunca van a vulnerar tu privacidad, porque les importa una mierda, ellos te proporcionan un sistema operativo cuyo desarrollo lleva siendo prácticamente el mismo durante casi 30 años y ya, si te gusta bien y si no pues ala.
Veo como algo bueno que a las entidades (en este caso el grupo de desarrollo de Debian) no les importe obtener tus datos, porque te da la garantía que en el futuro no van a intentar hacer cosas raras para monetizar el proyecto.

Éstas son mis opiniones sobre **Lo Bueno** en Debian, en el futuro pondré nuevos artículos explicando el resto de mis opiniones no tan buenas. 😈

Continuaré con la explicación en la parte 2: Debian Lo Feo.

Un saludo, [emilio.red](http://emilio.red) 😎