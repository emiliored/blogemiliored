---
title: "Debian Lo Feo"
date: 2024-09-05T22:20:06+02:00
author: "emilio.red"
description: "Mi opinión sobre el uso de Debian y sus características."
draft: false
---

Hola a todos, hoy comentaré mis pensamientos y opiniones sobre el sistema operativo Debian.

# Debian

Debian es un sistema operativo GNU/Linux que destaca su increible estabilidad, seguridad y rendimiento. Tanto es así que muchísimas distribuciones de Linux se basan en él. Debido a lo largo que es el artículo lo dividiré en tres partes. Ésta es la parte 2 de 3.

## Lo Feo

En este artículo procederé a explicar las partes tediosas sobre mi experiencia con Debian.

### La configuración

Es un coñazo, y ya. Vale me explico. La cosa de Debian es que te proporciona libertad absoluta, eso es algo bueno, pero si vienes de otros sistemas operativos, estarás acostumbrado a que esté todo mascadito, interconectado y que no tengas que hacer prácticamente nada, como ocurre con Windows o sistemas como Ubuntu. Eso en Debian no pasa, la configuración por defecto, no vale para mucho la verdad, te tendrás que tirar horas e incluso días configurándolo todo exáctamente como quieras, y al final, todo tiene su lado feo.

Te da mucha libertad, pero tienes que pasar mucho tiempo configurándolo todo y al final eres responsable de todo. Como ya comenté, si haces una mala configuración sabes que es tu culpa, que no hay otros factores externos. Por lo que, tienes que perder mucho tiempo pensando cómo hacer las cosas y cómo quieres que sean, por ejemplo:

- Puedes implementar una nueva configuración que te rompa el sistema operativo y te salga un Kernel Panic.

Tu puedes pensar, bueno, ha sido por negligencia del usuario, qué más da. Pero el problema es que debido a que la configuración por defecto es bastante inutil, tienes que meterte en un montón de problemas de configuración sólamente para salir a delante y tener un sistema operativo que no te de coraje usar. Ese tipo de "responsabilidad" o tedio, no lo tienes en otros sistemas operativos.

### Linux es de naturaleza descentralizada

Me explico, tu con Windows si tienes un problema, lo buscas en Google y sigues los pasos de páginas que te bombardean con publicidad. Al menos, sabes que seguramente esos pasos te puedan ayudar, porque en Linux, ya te aseguro que no tiene porqué.

En Linux, hay muchas distribuciones, muchos gestores de paquetes, muchas configuraciones diferentes, muchos entornos de escritorios diferentes, etc. Eso puede ser algo bueno, porque al final tienes la libertad de hacer tu Linux como tu quieras, el problema es que la mayoría de las veces no vas a entender todo en su plenitud. Eso significa, que puedes entender que tu tienes un driver de video instalado, y tienes un entorno de escritorio determinado, pero el error puede estar en el backend del entorno de escritorio que no ha sido adaptado correctamente a ese driver (como ocurre con Wayland y los drivers de Nvidia) y al final, no puedes culpar a nadie. 
- La comunidad a porteado un driver haciendo ingeniería inversa de Nvidia, 
- la comunidad ha creado y mantenido durante casi 30 años un backend de escritorio multipropósito (X11), 
- la comunidad a creado y mantenido un frondend de escritorio para que puedas usar tu sistema operativo con normalidad (por ejemplo KDE), 
- y los desarrolladores de tu distribución Linux te lo han juntado todo (En este caso el equipo de Debian).

Después de todo ese trabajo titánico que han hecho varias comunidades diferentes, a veces incluso de diferentes distribuciones de Linux (puede ser por ejemplo que no esté oficialmente soportado por tu distribución, pero puedas utilizar esas tecnologías), la única responsabilidad de todo recae sobre tí, nada ni nadie te garantiza que eso funcione, ni que cuando lo juntes todo funcione. Puede sonar fatalista, pero la teoría es ésta en realidad, y es lo que normalmente las comunidades de Linux no te cuentan.

En la práctica, los desarrollos y proyectos en Linux, creados por diferentes comunidades suelen ser muy muy muy buenos y profesionales. Normalmente todo se interconecta correctamente y no sueles tener problemas. El problema es cuando no es el caso (por ejemplo con los drivers propietarios).

#### Experiencia Nvidia

Si tienes una gráfica de Nvidia antígua (antes de la serie RTX 20xx, debido a que Nvidia hizo los drivers de código abierto), tarde o temprano vas a tener que instalarte los drivers propietarios de Nvidia. Sólamente te quedarás con los drives de Nouveau (el proyecto de ingeniería inversa que adaptó los drivers de Nvidia a Linux haciéndolos de código abierto) si estás dispuesto a desperdiciar la mitad de la capacidad de tu tarjeta gráfica, porque la mitad de las características no están implementadas a nivel software (a nivel de api), por ejemplo:
- Con el driver Nouveau no puedes tener la librería gráfica en 3D por lo tanto,
- Con el driver Nouveau no puedes jugar a juegos en Linux (sólamente a juegos 2D)

Y si tienes características especiales de tu gráfica, como por ejemplo, hacer uso de la librería de cálculo de Nvidia CUDA para aprovechar tu gráfica más allá de los videojuegos (por ejemplo puede ser que necesites calcular hashes o usarla para IA) si tienes los drivers de Nouveau olvídate.

Entonces es necesario instalarte los drivers propietarios si quieres aprovechar tu gráfica. El mayor problema de ello, es que a Nvidia le importa una mierda tener esos drivers actualizados y bien programados, es decir, ellos proporciona la ABI y la API donde los desarrolladores de otros proyectos pueden usar para comunicarse con la gráfica, pues como normalmente ocurre con este tipo de proyectos propietarios, se despreocupan, actualizan los drivers cuando quieren, si tienes un bug puede ser que nunca lo arreglen, etc. Dicho de otra manera Nvidia sólamente prioriza los drivers de Windows, y los de Linux pa' qué. Al menos siempre a sido así con Nvidia (no es algo novedoso) aunque con las nuevas gráficas no tengo ni idea (supongo que como es código abierto esto ya no debería pasar). Debido a la naturaleza descentralizada de los proyectos de Linux, la única garantía que tienes de que las cosas funcionen correctamente es que sean de código abierto, porque ni de broma Nvidia adaptará nada más allá de sus drivers.

Por lo tanto llegamos a la conclusión que comenté en apartados anteriores y es que siempre es mejor que todo sea de código abierto, porque no puedes confiar en ninguna empresa para que mantenga correctamente los proyectos.

En Debian siempre se ha dicho que la instalación de los drivers es intentar y probar, si tienes suerte funciona, sino a probar de otra manera. Si te ocurren varios Kernel Panic por el camino es tu problema, es tu responsabilidad arreglarlo, ya que al final **lo tienes que hacer todo por tu cuenta**.

### Hay algunos problemas que nunca podrás resolver

Este apartado tiene una cosa buena y una fea. Me explico:

Debido a que normalmente los drivers porteados a Linux son adaptaciones de Windows (normalmente de código abierto) su comportamiento es diferente. Según la ley de propiedad intelectual o Copyright, cualquier persona puede adaptar y hacer su propia versión de cualquier software (ya sea propietario o no) siempre que varíe en el código, es decir, sea una adaptación y no sea idéntico.

Pues bien, en Linux esas adaptaciones de drivers hacen que algunas veces se comporten de forma diferente que en Windows. Es decir, con el mismo hardware, el software y la experiencia de usuario es diferente, porque el firmware o drivers (que son las librerías utilizadas para comunicar el software y el hardware) es una adaptación y es por tanto diferente en Linux que en Windows.

Podrías pensar, bueno y qué más da. El caso es que eso supone nuevos problemas (bugs) o que la experiencia sea ligeramente diferente.

Por ejemplo:
- Mi driver de audio no normaliza el audio por lo que la experiencia de usuario es diferente. Noto como algunas veces los sonidos graves no los escucho y los agudos los oigo muy alto. Esto en Windows no pasaba, porque el driver o alguna librería hacía la normalización del sonido. Por lo tanto, con el mismo hardware, la experiencia de usuario es diferente debido a esa adaptación.
- Otro ejemplo son los codecs propietarios, en Linux por defecto no se encuentran instalados, por lo que algunas veces te encuentras que de repente se te estropea la experiencia en una página web porque el navegador necesita ese codec propietario para mostrar el contenido (podría usar otro codec equivalente de tu sistema, pero muchas veces no ocurre) y se peta la página.
- Mi ordenador tiene dos gráficas, una integrada de Intel y una dedicada de Nvidia. Cuando usaba Windows tenia un bug bastante molesto que trataba de cuando utilizaba la integrada, el ordenador no usaba la memoria de la dedicada la (VRam) y usaba la Ram del ordenador, por lo que había tirones en la reproducción del contenido. Pues bien, eso en Linux (Debian concretamente) no me pasa, ese error no lo tengo en Linux, eso es una maravilla por supuesto, pero me sirve para explicar el siguiente problema.

**Como los drivers son adaptaciones de software propietario y no se comportan igual, pueden surgir nuevos bugs o arreglarse bugs presentes en otros sistemas (porque los han parcheado en esa version o no existían en primer lugar) y tienes experiencias ligeramente diferentes** tienes que ser capaz de adaptarte y no frustarte.

### Especial agradecimiento

Después de todas estas quejas, he de admitir que Debian es mi sistema operativo favorito, me encanta, pero eso no hace que no tenga problemas. (Como todo en esta vida)
Mi intención no molestar ni ofender a nadie ni a ninguna comunidad. Es sólamente mi opinión sobre las experiencias que he tenido.
Tampoco quiero desprestigiar el trabajo asombroso que hacen estas comunidades sobre los infinitos proyectos de esta índole, soy consciente que es muchísimo esfuerzo y trabajo y encima gratis. Por eso, quiero agradecer a todas las personas y grupos presentes en estos proyectos, ya que ellos, son los que nos permiten tener esta libertad (de la que tanto me quejo). Muchas gracias de corazón.

Continuaré con la explicación en la parte 3: Debian Lo Malo.

Un saludo, [emilio.red](emilio.red) 😎