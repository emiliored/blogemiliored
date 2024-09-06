---
title: "Debian Lo Malo"
date: 2024-09-06T03:22:41+02:00
author: "emilio.red"
description: "Mi opinión sobre el uso de Debian y sus características."
draft: false
---

Hola a todos, hoy comentaré mis pensamientos y opiniones sobre el sistema operativo Debian.

# Debian

Debian es un sistema operativo GNU/Linux que destaca su increible estabilidad, seguridad y rendimiento. Tanto es así que muchísimas distribuciones de Linux se basan en él. Debido a lo largo que es el artículo lo dividiré en tres partes. Ésta es la parte 3 de 3.

## Lo Malo

Lo peor a destacar sería su complejidad. Algunos podeís pensar que hay otros sistemas operativos aún más tediosos de configurar y preparar (como Arch Linux) o incluso más complejos de entender y utilizar (como NixOS) pero eso no quita que Debian no es un sistema operativo para novatos.

A continuación explícaré más detenidamente lo que intento expresar, para simplificarlo un poco, yo he tenido dos experiencias con Debian:

1. Mi primera experiencia que fue un absoluto caos.
2. Mi segunda experiencia, que es la actual y es donde he aprendido a amar este sistema operativo.

### Mi primera experiencia

Debian no es un sistema operativo para novicios de Linux, te deja demasiada libertar, puedes contaminar el sistema operativo muy fácilmente con paquetes que son de otras subdistribuciones (como ocurre con los paquetes compilados para Ubuntu), y al no ser inmutable, si corrompes lo más mínimo el sistema o no sábes lo que estás haciendo en cada momento (por ejemplo, usando todo el rato el sudo o el usuario root), te encuentras con un sistema operativo muy complejo de arreglar los errores que has creado mientras intentas arreglar los errores que tenías en un principio. Eso hace que te puedas cargar el sistema operativo muy muy muy fácilmente. Al menos en Windows siempre hay una manera fácil de arreglar las cosas (normalmente). Por lo que yo seguiría las siguientes recomendaciones para que no te quedes noches enteras sin dormir, intentando arreglar un problema que has causado, porque has seguido una guía sin entender los comandos, y esa guía era para Ubuntu y tienes un sistema corrompido y completamente inestable.

#### Recomendaciones para utilizar Debian

1. Siempre saber qué hace exáctamente todos los comandos que ejecutas. Parece evidente, pero es dificil para un novicio saberlo, y puedes estudiar los comandos o preguntarle a algún ChatBot como ChatGPT.
2. Si no te convence alguna guía que veas en internet, no la sigas. Porque si lo haces te puedes cargar tu sistema muy fácilmente. Como decimos en España: "Es peor el remedio que la enfermedad."
3. No uses el usuario **root**, ponlo con el nologin, y usa el **sudo** como sustituto. Esta es una medida importante de seguridad.
4. Aprende a usar el firewall para hacer de tu ordenador más seguro. Si no quieres aprenderte las tablas arp, puedes utilizar **UFW** que es muy bueno (el único problema que tiene es que no puedes configurar la capa de red, las peticiones ping, etc).
5. Para tu primera distro Linux no deberías usar Debian, utiliza una distribución inmutable como VanillaOS, debido a que si te cargas el sistema operativo (que lo vas a cabar haciendo) puedas arreglarlo en segundos y no en una noche entera (con suerte).
6. Antes de cambiar a Debian busca sustituto de tus aplicaciones que utilizas en Windows y/o Mac. Porque la inmensa mayoría (a excepción de los juegos) no vas a poder usarlos.
7. Muchas de las deficiencias de Linux se pueden arregar usando una máquina virtual con Windows. No sientas pudor al usar un Windows, no hace falta ser un purista de Linux.
8. Si te sientes abrumado/frustado siempre puedes volver a un sistema operativo con el que te sientas cómodo. Puedes intentarlo más adelante. Aunque recuerda que del esfuerzo se aprende.
9. Todos los que usamos Debian sabemos que si alguna vez ocurre un problema nos podemos tirar horas intentando arreglarlo. Por eso se suele modificar las cosas poquito, como en las empresas hacen con los servidores.
10. Las actualizaciones oficiales de Debian **nunca** van a romper el sistema operativo, así que no tengas miedo al actualizar (cosa que sí ocurre en Arch o en Windows).

La mayoría de recomendaciones que he indicado anteriormente se pueden aplicar a Linux en general y no sólamente a Debian.
Éstas son algunas de mis recomendaciones, en un futuro intentaré explicar más (para no extender este artículo demasiado).

### Mi segunda experiencia

Cuando ya tienes un conocimiento intermedio de Linux, es muy gratificante. Tienes un sistema operativo estable complétamente configurado a tu gusto. A diferencia de mi primera experiencia, ahora si lo he disfrutado el camino completo, tanto que usaré Debian a partir de ahora y no me cambiaré a otro sistema operativo.

### Las actualizaciones son lentas

Acostúmbrate a ello, a diferencia de Windows y Arch que se actualizan prácticamente todos los días, Debian lo hace normalmente 2 o 3 veces al mes. Normalmente esas actualizaciones son de seguridad. Ya que al equipo de Debian no le da tiempo a testear completamente todos los programas antes. Aunque eso me parece algo bueno, es una garantía. Si yo actualizo el sistema se que no se va ha desconfigurar nada ni ha desestabilizar el sistema.

La mayoría de veces que actualizo el sistema operativo, las actualizaciones son para las aplicaciones Flatpak.

### Especial agradecimiento

Después de todas estas quejas, he de admitir que Debian es mi sistema operativo favorito, me encanta, pero eso no hace que no tenga problemas. (Como todo en esta vida)
Mi intención no molestar ni ofender a nadie ni a ninguna comunidad. Es sólamente mi opinión sobre las experiencias que he tenido.
Tampoco quiero desprestigiar el trabajo asombroso que hacen estas comunidades sobre los infinitos proyectos de esta índole, soy consciente que es muchísimo esfuerzo y trabajo y encima gratis. Por eso, quiero agradecer a todas las personas y grupos presentes en estos proyectos, ya que ellos, son los que nos permiten tener esta libertad (de la que tanto me quejo). Muchas gracias de corazón.

En un futuro intentaré explicar más experiencias y peripecias con Debian. 😊

Con esta trilogía doy por terminada mi opinión sobre Debian. Como habéis podido intuir es mi sistema operativo favorito, me encanta aún con todos sus defectos. ❤️

Un saludo, [emilio.red](emilio.red) 😎