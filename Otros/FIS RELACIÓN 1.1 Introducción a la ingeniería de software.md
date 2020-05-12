# FIS RELACIÓN 1.1: Introducción a la ingeniería de software 

###### Clara María Romero Lara

### 2. ¿Qué diferencias existen entre las distintas clases de Software según los derechos de autor? Proponga ejemplos de programas de las distintas clases.

- **Código abierto:** puedes ver el código del programa que utilizas. En el caso de programas de pago, como comprador se considera tu derecho el ver el código que usas e incluso modificarlo y redistribuirlo según tus necesidades y el tipo de licencia.
  - Distribuciones Linux como Arch, Ubuntu, Debian... Suite Open Office y Libre Office...
- **Código cerrado:** el código del programa no es visible bajo ningún concepto. Sólo el desarrollador puede verlo y alterarlo, cómo usuario no hay forma de saber qué hace exactamente el programa.
  - Windows, Skype, Suite Adobe...
- **Dominio público:** al igual que en el caso de software libre, puedes acceder al código del programa. El uso, modificación, y redistribución es totalmente libre, al contrario que el anterior que dependía de la licencia.
  - UNIX

### 4. Ponga dos ejemplos de mito del Software y explique brevemente su significado y las diferencias entre el mito y la realidad.

>***MITO:***
>
>*"La ingeniería de software hará que generemos documentación voluminosa e innecesaria, e invariablemente nos retrasará."*

**REALIDAD:**

El producto de la ingeniería de software no son los documentos, sino el sowftare en su totalidad, lo cual incluye la documentación. Una buena documentación crea un producto de calidad y facilita el trabajo posterior sobre este.

> ***MITO:***
>
> *"Si nos atrasamos, podemos agregar más programadores y ponernos al corriente"*

**REALIDAD:**

Incorporar más gente a un proyecto no hace que este se acabe más rápido, al contrario. Los desarrolladores que ya estaban trabajando en el programa desde el inicio paran su producción para explicar a los que han entrado nuevos y el tiempo se alarga.

### 5.El cuarto principio del código de Ética y práctica Profesional de la Ingeniería del Software del ACM y del IEEE-CS dice: 

> *“Los ingenieros de software deben mantener la integridad e independencia en sus juicios profesionales”*. 

### Explique el significado que, a su juicio, puede tener este principio. Proponga un ejemplo de posible aplicación del mismo. Busque más información sobre códigos éticos y de profesionalidad en la Ingeniería del Software. ¿Piensa que este tema tiene algún interés o utilidad?

El desarrollador debería siempre dar soluciones correctas (o lo más correctas posibles a su juicio) sin verse influenciado por motivos externos (p.ej. malintencionadamente fallar en algún punto del proceso para que se sigan requiriendo sus servicios).

Los 8 principios de la ética y práctica profesional de la IS son:

- *Sociedad*: Los ingenierios de software actuarán de manera coherente con el interés social.
- *Cliente y Empresario*: los ingenieros de software actuarán de manera que produzca el mejor resultado para cliente y empresario, y de manera coherente con el interés social.
- *Producto*: los ingenieros de software garantizarán que sus productos y las modificaciones correspondientes cumplen los mayores estándares profesionales posibles.
- *Valoración*: los ingenieros de software mantendrán la integridad e independencia en sus valoraciones profesionales.
- *Gestión*: los líderes y gestores de ingeniería de software suscribirán y promoverán un enfoque ético en la gestión del desarrollo y mantenimiento del software.
- *Profesión*: los ingenieros de software avanzarán en la integridad y reputación de la profesión, de manerar consistente con el interés social.
- *Compañeros*: los ingenieros del software serán justos y apoyarán a sus compañeros.
- *Personal*: los ingenieros del software participarán en el aprendizaje continuo referente a la práctica de su profesión y promoverán un enfoque ético en la práctica de la profesión.

Estos principios son útiles para el campo y la sociedad, ya que si se mantiene una buena ética profesional el desarrollo y evolución serán favorables (para buenos fines) y correctos (se hace el mejor trabajo posible).

### 6. ¿Cómo piensa que puede afectar a la gestión de los proyectos software el carácter lógico del mismo?

El caracter lógico de los proyectos afecta a todas las partes del desarrollo: un programa difícil a nivel lógico llevará más tiempo de análisis, mayor esfuerzo y  más tiempo de desarrollo. 

Hay que tener en cuenta no sólo la dificultad inherente al problema sobre el que se trabaja, sino que, incluso dado un buen análisis, el hecho de desarrollarlo conlleva esfuerzo y tiempo para la corrección de el mismo - ya sea a nivel de implementación o de análisis.

No obstante, se cuenta con la ventaja de que son proyectos cuyos requisitos físicos o materiales son escasos por parte del desarrollador y de alto grado de reutilización (p.ej. un servidor puede servir para varios proyectos)

### 7. Considere uno de los proyectos siguientes y haga una estimación del esfuerzo necesario, así como de los costos y del plazo de entrega. Seleccione el modelo de proceso que mejor se adapta al proyecto. Compare sus estimaciones con las que realicen otros compañeros.

- **Gestión de una ONG de integración social de colectivos marginados** 
- ***Gestión de una Biblioteca***
- **Gestión y control de unas instalaciones deportivas** 
- **Aplicación de seguridad para unos grandes almacenes** 
- **Un juego de 3 en raya para Android** 
- **Un editor de texto html** 
- **Cualquier otro de su elección**

Es un proyecto cuyas estimaciones variarán según el tamaño de la misma y su sistema interno de trabajo, pero tomamos de ejemplo una biblioteca de tamaño medio-grande.

Habrían de desarrollarse bases de datos para los múltiples servicios que puede ofrecer una biblioteca de estas prestaciones:

- Biblioteca
- Hemeroteca
- Videoteca
- Meloteca

Es un proyecto que implica **mucho trabajo repetitivo** de documentación para estas bases de datos, **pero relativamente simple a niveles de implementación**: aunque haya desarrollar multiples bases de datos, las funciones que estas ejecutan entre sí son prácticamente iguales. Además es un proyecto que **no conlleva altos riesgos** de seguridad ciudadana, sólamente a nivel económico-material y a una muy baja escala que se pueden subsanar con multas y penalizaciones.

Un modelo a utilizar podría ser el **modelo incremental**, con énfasis en el aspecto de comunicación incial para saber perfectamente el sistema de préstamos y catálogo de esta biblioteca: una vez planteado un programa de préstamos base es sencillo ir implementando los diferentes servicios ofrecidos.

**Respecto al coste y entrega, es proporcional al tamaño del equipo** de desarrollo. Si estamos asumiendo que esta biblioteca no disponía de ninguna base de datos digital previa, y un equipo de trabajo mediano documentándola, podríamos estimar un mes para la base de datos y otro mes para la implementación del sistema.

### 9. La “alianza Ágil” deﬁnió una serie de 12 principios que debería tener una metodología para alcanzar niveles aceptables de agilidad. Puede encontrar estos principios en el enlace que aparece en el ejercicio 1. Comente los problemas que intenta solucionar alguno de estos principios. 

> Entregamos software funcional frecuentemente, entre dos semanas y dos meses, con preferencia al periodo de tiempo más corto posible. 

Se soluciona el problema de "hasta que no tenemos un código funcional, no podemos saber cómo va el proyecto". Basándose en un modelo evolutivo, las versiones funcionales existen desde el principio, así que se puede comprobar el avance del proyecto. 

> El método más eﬁciente y efectivo de comunicar información al equipo de desarrollo y entre sus miembros es la conversación cara a cara. 

No sólo conversación cara a cara, sino a ser posible contar con una pizarra o similar. De este modo se evitan muchos malentendidos respecto a los requisitos y el desarrollo. 

> El software funcionando es la medida principal de progreso. 

Muy similar a uno de los puntos anteriores: el software en funcionamiento desde el inicio permite aplicar los cambios y correcciones necesarios de forma gradual, mucho mejor que tener que corregir todo desde el principio 

> La atención continua a la excelencia técnica y al buen diseño mejora la Agilidad. 

Facilita la evolución del proyecto: un buen código, bien diseñado e implementado, con correcta documentación, etc. ("excelencia técnica") permite trabajar sobre el proyecto con conocimiento y lo hace accesible a otros desarrolladores de nuestro equipo o externos.