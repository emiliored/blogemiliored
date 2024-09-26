---
title: "🔥 Bienvenidos a mi blog 🔥"
date: 2024-09-03T04:05:28+02:00
author: "emilio.red"
description: "Breve introducción y consideraciones varias"
draft: false
---

# Hola a todos
En esta entrada de blog explicaré mis ambiciones y mis objetivos con este blog y la página.

# Contexto
Recientemente he comprado el dominio [emilio.red](https://emilio.red) y busco crear una imagen de mía en internet que me permita desarrollar mis intereses sin tener que ceder mi privacidad y seguridad por el camino, me explico.

## Privacidad
Al hacer uso del nuevo dominio puedo utilizar nuevos álias de correo que me permitan enmascarar mi dirección de correo real, en la cúal la estoy intentando centralizar; con centralizar, me refiero a que antes tenía varias cuentas de correo distintas que me servían para "filtrar" un poco los correos. El problema de aquello es que era un caos porque no sabía exactamente qué cuentas estaban asignadas a qué correos (este hecho es importante, lo explicaré en el siguiente apartado).

### Filtración de datos en cuentas y el robo de éstas
Cuando te creas una cuenta en internet siempre y digo SIEMPRE tienes que suponer que se va a filtrar la base de datos del servidor de la cuenta y prácticamente tus datos se harán públicos.
Mi experiencia en el desarrollo de Backends me ha enseñado que aunque no es un proceso complejo (el hacer que el servidor siga estándares de seguridad de la industria), prácticamente ningún servicio en internet lo respeta porque es un proceso tedioso. 

Hay numerosos casos de filtraciones de datos como por ejemplo:
- Las numerosas filtraciones de Lastpass: [FuenteEjemplo](https://www.redeszone.net/noticias/seguridad/gestor-contrasenas-lastpass-filtracion-datos/)
- Filtraciones como la de Twitch (que filtró no solamente código de backend, sino también datos financieros de los streamers): [FuenteEjemplo](https://vandal.elespanol.com/noticia/r12740/la-gran-filtracion-de-twitch-esto-es-lo-que-ganan-auronplay-ibai-thegrefg-o-rubius)

Y podría seguir poniendo más ejemplos (hay infinidad de casos parecidos) pero sinceramente me da pereza.

Aunque en un futuro me encantaría poner una guía de cómo obtener filtraciones de datos usando la red I2P (hay muchas maneras más sencillas, pero cuando aprendí los conceptos de la red I2P me fascinaron).

### Organización de los correos y las cuentas mediante alias de correo
Debido a lo anteriormente explicado, se me hizo necesario crear dichos alias de correo. Estoy utilizando Cloudflare para ello, por la comodidad y lo barato que es la verdad. Se que algunas personas piensan que Cloudflare también es una espada de Damocles en lo que se refiere a la privacidad, pero la verdad, no le doy mucha importancia.

En mi proyecto y mis casos de uso lo veo útil y necesario. De esta manera puedo filtrar mediante reglas (filtros en Thunderbird) de correo (en Outlook) los correos que recibo mediante los alias asignados, de tal manera que van directamente a Spam, a carpetas temporales, al buzón, etc.

De esta manera mantengo una máscara (el alias de correo) entre el emisor y yo. Sólamente descubren mi correo real si así lo deseo, garantizando mi privacidad.

### Los dominios personales son menos receptivos a baneos
Me explico:
- Un día cuando estaba en la universidad, utilicé un proxy para intentar saltarme el Firewall, y la única razón por la que fallaba, era porque no podía resolver la petición DNS del dominio porque estaba utilizando un dominio público gratuito en internet, que dicho dominio es ampliamente conocido y al banear ese dominio, mi subdominio era baneado también.
- Tardé bastante en darme cuenta, aunque es un problema bastante tonto la verdad, porque diréctamente te conectas desde la IP de tu proxy y ala, funciona, pero este tipo de cosas lo suelen ofuscar bastante en los Firewall para que te des por vencido y lo dejes.
- El proxy funcionaba perféctamente y si hubiese utilizado un dominio personal, no me habría pasado.

En un futuro explicaré mis aventuras y cómo conseguí saltarme el Firewall fácilmente y de diferentes maneras en la universidad.

## Seguridad
### Uso de Hugo
Utilizar Hugo (el generador de páginas web estáticas que he utilizado para que leas este artículo) es necesario porque me permite:
- Mantener la seguridad en la página y en el blog, al no haber nada dinámico ni ningún motor (como podría ser Wordpress por ejemplo) la única información que pueden obtener es la que publique con Hugo (evidentemente la idea es que sólamente publique lo que quiera publicar, por lo tanto es público).
- Me permite crear páginas web con cierto grado de dinamismo completamente gratis. Esta página web está siendo alojada en Cloudflare gratis (sólamente pago el dominio).
- Puedo crear infinidad de páginas web utilizando esta tecnología para diferentes ámbitos, ya que su alojamiento y la creación de los subdominios es completamente gratis.

### Clave PGP Pública
He colgado mi clave PGP pública en la página (pgp.emilio.red), para que la gente que quiera contactar a mi correo pueda cifrar los mensajes, de tal manera que se garantiza la privacidad de los mismos, la seguridad en la autenticación y la seguridad de que sólamente lo lee el destinatario.

Sientete libre de enviarme correos cifrados a la dirección pública [contactar@emilio.red](mailto:contactar@emilio.red)

### Independencia Tecnológica
Éste es un apartado complejo y el que me gustaría explayarme en un futuro, pero básicamente el uso de estas tecnologías y el dominio me permite controlar exáctamente cómo se utilizan, qué hacen y con qué propósito.
- Garantizando que los datos publicados y sus servicios sean agnósticos de la plataforma. Como por ejemplo el uso de alias de correo me permite elegir que proveedor utilizar y cambiarlo en cualquier momento.
- Los datos publicados en Hugo pueden ser fácilmente adaptados a otros sistemas y/o servicios como Wordpress, etc.

# Objetivos
En esta introducción del blog he hablado un poco de todo, de mis pensamientos y razonamientos para el uso de éste. De eso tratará esta página espero que te guste y aguardes con ansias mis próximas entradas, ya que intentaré hacer guías de numerosas tecnologías que he ido utilizando y aprendiendo a lo largo de los años, y explicaré detallamente el por qué de su uso, y en qué se diferencian de la competencia.

Un saludo, [emilio.red](http://emilio.red) 😎