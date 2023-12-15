



# Tarea UD2 - Determinación del nivel de seguridad requerido por las aplicaciones #

**Juan Martínez Gómez**



### Índice

1. Enunciado
2. Introducción
3. Análisis de la vulnerabilidad
4. Situaciones donde se puede dar
5. Escenario



### 1. Enunciado ###

**Contexto práctico**

Debes realizar un trabajo individual sobre una de las vulnerabilidades recogidas por la OWASP, que te asignará el profesor (**Fallos en el registro y Monitoreo**). Pueden ser tanto vulnerabilidades web como vulnerabilidades móvil.

El trabajo debe constar de un índice, una introducción, un análisis de la vulnerabilidad, un apartado donde expliques 3 situaciones donde se pueda dar y un escenario donde pongas en práctica una de las situaciones, de manera práctica, realista y simulada. Por un lado, debes documentarte y analizar la vulnerabilidad. Una vez realizado esto, debes reproducir la vulnerabilidad asignada de forma que se perciba cómo esta afecta, qué es lo que la caracteriza y, para finalizar, como se puede solventar desde tu punto de vista.

Para esta entrega puedes realizar un trabajo escrito para la parte teórica y luego realizar un video mostrando la vulnerabilidad, reproduciéndola en tu equipo. En caso de no realizar un video mostrándola, debes documentar paso a paso y haciendo evidente qué quieres mostrar, de una situación de la vulnerabilidad asignada.

**¿Qué se pide?**

1. Realizar un trabajo en formáto ánalisis de la vulnerabilidad. Debe contener mínimo: índice, introducción, análisis de la vulnerabilidad, 3 escenarios actuales y realistas donde suceda o pueda suceder.
2. Entregar una reproducción, integrándola en el markdown (.md), ya sea en formato video o documentación, donde reproduzcas un escenario en tu propio equipo/nube/vm/contenedor donde se dá la vulnerabilidad.



### 2. Introducción ###

Dentro de los recursos que tienen los profesionales de la informática y las empresas para fortalecer la seguridad informática, existe uno que se ha convertido en crucial para el sector, el **Top 10 de vulnerabilidades y fallos de seguridad** más críticos del momento. Esta publicación de la **OWASP** (Open Web Application Security Proyect) aprovecha el potencial de las fuentes abiertas para evaluar distintos parámetros como vulnerabilidades, ataques conocidos, impactos y manejo de datos, y gracias a ello poder hacer la clasificación de las vulnerabilidades web. La importancia de este Top10 no solo radica en servir de guía para identificar y mitigar riesgos, también juega un papel educativo y de sensibilización importante al destacar mejores prácticas de seguridad en el desarrollo del software.

Además de una lista de problemas de seguridad, el Top10 de OWASP también es un reflejo de hacia a dónde avanza el mundo de la seguridad informática. Cada punto de la lista es resultado de una profunda compilación y análisis de datos, junto con contribuciones de muchos expertos en seguridad y consultas a la comunidad de desarrolladores que hacen de esta lista un termómetro de los desafíos del sector.

En este trabajo nos centraremos en uno de los puntos de la lista, concretamente el que está en novena posición, **Fallos en el registro y monitoreo**. Haremos un análisis de esta vulnerabilidad, estudiando posibles escenarios. 



### 3. Análisis de la vulnerabilidad ###

**Fallos en el registro y monitoreo** ocupa actualmente la novena posición del Top10 de OWASP. Hace referencia a la insuficiencia o ineficacia de los mecanismos de registro y monitoreo de las aplicaciones, lo que puede provocar que no se detecten ataques o fallos de seguridad. Es una vulnerabilidad crítica, porque un sistema robusto que analice y monitorice la seguridad es esencial para poder detectar y responder ante ataques. 

Las herramientas de registro y monitoreo nos ayudan a identificar patrones inusuales sospechosos, señales de que se puede estar produciendo un ataque o una falla de seguridad. Son importantes porque sin ellas será muy difícil detectar el peligro, y mucho menos hacerle frente. No saber qué parte del sistema es vulnerable para arreglarla por desconocer incluso que ha habido un ataque por esa parte.

![ladron](img/ladron.jpg)

_Cuando un ladrón entra en una casa particular, tiene primero que pisar el césped, abrir una ventana, desplazarse por la casa, perder tiempo examinando lo que se puede llevar, salir, etc. En todo ese proceso puede hacer ruido, dejar huellas de barro o cosas movidas de sitio, señales de que algo no va bien, pero seríamos incapaces de detectar todo eso si nadie comprueba el estado del césped, ni si las ventanas están correctamente cerradas, ni hace un inventario de las cosas que tiene junto con la comprobación de que las tiene todas. Si nadie tampoco observa las huellas de barro para determinar por qué ventana entraron, ni se para a analizar por qué hay un hueco donde antes había algo, el ladrón podría volver a repetir su hazaña todas las veces que quisiese porque nadie tendría manera de darse cuenta, **sería una casa muy vulnerable**, aunque contase con todo tipo de armas para hacer frente a un potencial ladrón._



Las consecuencias de esta vulnerabilidad son bastante importantes, se tarda más tiempo en detectar una brecha de seguridad, si es que se detecta, habiendo también imposibilidad de hacer un seguimiento adecuado a las señales sospechosas. Derivado de esto estaría la incapacidad de encontrar puntos vulnerables en el sistema al no poder realizar de forma adecuada una auditoría. Por último estaría el apartado de la normativa, donde seguro se incumpliría en muchos casos, lo que podría conllevar multas.

Para solventar esta vulnerabilidad se pueden aplicar buenas prácticas, como por ejemplo implementar un sistema de registro, 

