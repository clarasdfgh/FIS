# FIS TEMA 1: Introducción a la ingeniería de software

### 1.El producto software

#### Definición y tipos de software

Programa o conjunto de programas de cómputo que incluye datos, procedimientos y pautas que permiten realizar distintas tareas en un sistema informático.

Es un transformador de información. Para ello adquiere, gestiona, modifica, transmite o produce información.

> Software == Programa de computadora

Podemos clasificarlo según:

- **Su campo de aplicación**
  - Software de sistemas
  - Software de aplicaciones
  - Software de programación
- **Tipo de licencia**
  - *Según derechos de autor*
    - Código abierto
    - Código cerrado
    - Dominio público
  - *Según destinatario*
    - Usuario final (software a medida)
    - Distribución (software genérico)

#### Características principales

1. El software es un producto lógico: se **desarrolla** (no se *fabrica*), se **deteriora** (no se *estropea*). Según lo desarrollamos, los errores vienen y van, no es la curva idealizada

   ![image-20200217161226198](/home/clara/.config/Typora/typora-user-images/image-20200217161226198.png)

2. El software crea **modelos de la realidad.** Representamos algo de la realidad, pero no es real. Los modelos simplifican la realidad, pero pueden generar sesgos o ser incorrectos

   *Por ejemplo, en el desarrollo de interfaces de usuario un developer puede creer que la interfaz queda clara al usuario pero que no sea así*

3. El software está formado por múltiples piezas que deben encajar entre sí perfectamente

#### Proceso de producción

![image-20200217161933426](/home/clara/.config/Typora/typora-user-images/image-20200217161933426.png)

![image-20200217162751029](/home/clara/.config/Typora/typora-user-images/image-20200217162751029.png)

- **DEFINICIÓN:** el *"¿Qué?"* del problema. Es donde pueden surgir los mayores fallos. Entender las circunstancias, condiciones, requisitos, limitaciones...

  - Ingeniería de sistemas
  - Ingeniería de requisitos
  - Planificación de proyectos

- **CONSTRUCCIÓN:** el *"¿Cómo?"*. No es sólo la implementación, es también el estudio de cómo lo vamos a aplicar. Incluye rectificar la definición.

  - Diseño del software
  - Generación del código
  - Prueba del software

- **EVOLUCIÓN:** los cambios tras las fases anteriores. El seguimiento a posteriori.

  - Corrección

  - Adaptación

  - Mejora

  - Prevención

    <img src="/home/clara/.config/Typora/typora-user-images/image-20200217162812551.png" alt="image-20200217162812551" style="zoom:80%;" />

#### Problemas en el desarrollo

1. **COMUNICACIÓN ENTRE PERSONAS:** entender correctamente al cliente, coordinarse con el resto de desarrolladores, seguir el diseño...

2. **INCUMPLIMIENTO DE LA PLANIFICACIÓN:** no estimar correctamente los plazos, errores derivados de la comunicación entre personas...

   A veces se intenta solucionar metiendo más desarrolladores *(horda mongoliana)*, pero no es sino más espacio a problemas de comunicación

3. **INCORPORAR CAMBIOS EN ETAPAS AVANZADAS: ** el impacto de los cambios aumenta con el avance del proyecto

   <img src="/home/clara/.config/Typora/typora-user-images/image-20200217163711476.png" alt="image-20200217163711476" style="zoom:80%;" />

### 2.Concepto de ingeniería de software

#### Necesidad de la ingeniería del software

- Calidad (mal funcionamiento)
- Mantenimiento del software existente
- Demanda de nuevo software
- Adaptación a nuevas tecnologías
- Incremento de la complejidad

![image-20200217164312667](/home/clara/.config/Typora/typora-user-images/image-20200217164312667.png)

#### Definición de ingeniería del software

Bauer, 1972:

> Establecimiento de los **principios y métodos de la ingeniería** a fin de obtener software de modo rentable que sea fiable, y trabaje en máquinas reales. 

Bohem, 1976:

> Aplicación práctica del conocimiento científico en el diseño y construcción de programas de computadora, y la **documentación** asociada y requerida para el desarrollo, operación y **mantenimiento** del programa.

Zelkowitz, 1978:

> Estudio de los **principios y métodos** para el desarrollo y mantenimiento de sistemas software.

Standard IEEE, 1993:

> Aplicación de un **enfoque sistémico**, disciplinado y cuantificable al desarrollo, operación y mantenimiento del software; es decir, aplicación de la ingeniería al software.

Marré, 2002:

>Conjunto de **teorías, métodos e instrumentos** (tecnológicos y organizativos) que permitan construir sistemas software con las características de **calidad** deseadas.

Sommerville, 2011:

> Disciplina de ingeniería que se interesa por **todos los aspectos de la producción de software,** desde las primeras etapas de la especificación hasta el mantenimiento del sistema después de su puesta en operación.

#### Terminología de ingeniería de software

- **Sistema:** conjunto de elementos relacionados entre sí y con el medio, que forman una unidad o todo organizativo

  - **Sistema basado en computador:** conjunto o disposición de elementos organizados para cumplir una meta predefinida al procesar información

    <img src="/home/clara/.config/Typora/typora-user-images/image-20200217165408361.png" alt="image-20200217165408361" style="zoom:80%;" />

  - **Sistema software:** conjunto de piezas o elementos software relacionados entre sí y organizados en subsistemas

    <img src="/home/clara/.config/Typora/typora-user-images/image-20200217165504420.png" alt="image-20200217165504420" style="zoom:80%;" />

- **Modelo:** representación de un sistema en un determinado lenguaje. De un mismo sistema pueden surgir muchos modelos

- **Principio:** elementos adquiridos mediante el conocimiento que definen las características que debe poseer un modelo para ser una representación adecuada de un sistema

- **Herramienta:** instrumentos que permiten la representación de modelos

- **Técnica:** modo de utilización de las herramientas

- **Heurística:** conjunto de reglas empíricas que, al ser aplicadas, producen modelos que se ajustan a los principios *(ej. No usar materiales flexibles a la hora de hacer una maqueta de un edificio)*

- **Proceso:** estructura que debe establecerse para la obtención eficaz de un producto de ingeniería

- **Método:** proporcionan la experiencia ténica para elaborar el producto software, se basan en principios fundamentales e incluyen actividades de modelado

![image-20200217165859665](/home/clara/.config/Typora/typora-user-images/image-20200217165859665.png)

- **Ingeniería del Software:** estudio de los principios, metodologías y herramientas que forman parte de un proceso para facilitar el desarrollo y mantenimiento de sistemas software de calidad

### 3.Proceso de desarrollo de software

#### Concepto del proceso de desarrollo

El proceso de desarrollo de software incluye al conjunto de actividades, acciones y tareas que se realizan cuando va a crearse un producto o sistema software

- **Actividad:** busca el logro de objetivos amplios e independientes del tipo de aplicación a desarrollar y de su complejidad
  - *Ej. planificación del proceso de desarrollo*
- **Acción:** conjunto de tareas que producen un producto importante como resultado
  - *Ej. modelado de la arquitectura del sistema software*
- **Tarea:**  objetivo pequeño y bien definido que produce un resultado tangible
  - *Ej. realizar una prueba unitaria*

Este esquema permite un enfoque adaptable, basado en el número mínimo de actividades y en el que cada equipo de desarrollo define el conjunto de acciones y tareas que forman parte de cada actividad.

##### Tipos de actividades

- **Estructurales:** dedicadas a obtener el producto
  - Comunicación: colaboración con el cliente para entender objetivos y requisitos del proyecto
  - Planificación: definir el plan del proyecto en el que se describen los riesgos probables, los recursos necesarios, los productos obtenidos y se programan las actividades, tareas y acciones
  - Modelado: representación mediante modelos del sistema propuesto junto con la solución o soluciones apropiadas
  - Construcción: generación del código y su prueba
  - Despliegue: entrega al consumidor y evaluación por parte de éste, la cual sirve de retroalimentación para el equipo de desarrollo
- **Sombrilla:** se aplican a lo largo de todo el proceso
  - Seguimiento y control del proyecto
  - Administración del riesgo
  - Aseguramiento de la calidad
  - Revisiones técnicas
  - Mediciones de parámetros del proceso
  - Administración de la configuración
  - Administración de la reutilización
  - Preparación y producción del producto de trabajo

#### Modelo de proceso

##### Modelo general de proceso

Cada una de las actividades, acciones y tareas se encuadran dentro de una estructura que define su relación con el proceso y entre ellas. Un esquema general de la estructura de proceso sería el siguiente:

<img src="/home/clara/.config/Typora/typora-user-images/image-20200622180512635.png" alt="image-20200622180512635"  />

El **flujo del proceso** describe la manera en la que se organizan las actividades estructurales, acciones y tareas dentro de cada uno con respecto a la secuencia y el tiempo. Los siguientes esquemas se muestran distintos flujos de proceso:

![image-20200622182125740](/home/clara/.config/Typora/typora-user-images/image-20200622182125740.png)

![image-20200622182136646](/home/clara/.config/Typora/typora-user-images/image-20200622182136646.png)

![image-20200622182147764](/home/clara/.config/Typora/typora-user-images/image-20200622182147764.png)

###### Acciones y tareas de las actividades estructurales:

- Obtención de requisitos: indagación para obtener información sobre qué es lo que se espera del software
- Estimación y planificación del proyecto: estimar tiempo y costes del desarrollo
- Análisis de requisitos: análisis del problema a resolver. Documento en el que se dice qué debe hacer el sistema software
- Diseño: búsqueda de la solución. Descripción de componentes, sus relaciones y funciones que dan solución al problema
- Implementación: traducción del diseño a un lenguaje de programación entendible por la máquina
- Prueba de Software: revisión y validación de todo el código que se va desarrollanod
- Evaluación y aceptación: evaluación del producto y aceptación por parte de los interesados en el sistema software
- Entrega y asistencia: el sistema está operando y asistencia para su correcto funcionamiento

##### Modelo en cascada

![image-20200217170941095](/home/clara/.config/Typora/typora-user-images/image-20200217170941095.png)

- Características generales:
  - Estructura secuencial y proceso de flujo lineal
- Problemas que presenta:
  - Los proyectos reales difícilmente se adecuan a este modelo
  - Dificultad para expresar por parte del cliente todos los requisitos al inicio del proyecto
  - Poca comunicación con cliente/usuario, hasta las etapas finales no existe un ejecutable a evaluar

##### Modelo incremental

![image-20200622202817708](/home/clara/.config/Typora/typora-user-images/image-20200622202817708.png)

- Características generales:
  - Estructura secuencial y flujo de proceso lineal y paralelo entre incrementos 

##### Modelos evolutivos

Los modelos evolutivos son iterativos y nacen de la exigencia de tiempo de entrega muy limitado, la necesidad de facilitar la incorporación de cambio y de satifacer al usuario/cliente. En cada iteración del proceso se obtiene un producto terminado y operativo

- Características generales:
  - Afrontan los riesgos altos (técnicos, de requisitos, usabilidad...) tan pronto como sea posible
  - Retroalimentación temprana por parte del usuario
  - Manejo de la complejidad (pasos cortos y sencillos)
  - El conocimiento adquirido durante una iteración de la evolución se acumula para las siguientes
  - Involucra continuamente al usuario

###### Modelo de prototipos

Un prototipo es una representación limitada de un producto que se utiliza para probar las opciones de diseño y para comprender mejor el problema y sus posibles soluciones, o un producto de funcionamiento limitado en cuanto a su capacidad, confiabilidad o eficiencia 

Tipos de prototipos: 

- **Prototipo evolutivo:** Como producto final 
- **Prototipo desechable:** usados dentro de otros modelos de proceso

![image-20200622205612074](/home/clara/.config/Typora/typora-user-images/image-20200622205612074.png)

- Se usa para:
  - Facilitar la obtención y validación de requisitos (desechable)
  - Estudios de viabilidad (desechable)
  - Propuestas de soluciones (diseños) alternativas (desechable)
  - En casos muy concretos como producto final (evolutivo).
- Inconvenientes:
  - Crea falsas expectativas por parte del cliente/usuario (desechable)
  - Decidir qué partes del diseño del prototipo pasan a formar parte del producto final (evolutivo)

###### Modelo iterativo en espiral de Boehm

![image-20200623180542160](/home/clara/.config/Typora/typora-user-images/image-20200623180542160.png)

- Características:
  - Centrado en el análisis de riesgo, haciendo uso de construcción de prototipos para su estudio
  - La espiral puede continuar una vez finalizado todo el proceso y entregado el producto para llevar a cabo la etapa de mantenimiento
  - Es un enfoque adecuado para el desarrollo de sistemas a gran escala
- Inconvenientes: 
  - Modelo de proceso predictivo no adaptable a la complejidad ni al tipo de sistema
  - Requiere un equipo de desarrollo con gran experiencia en análisis de riesgo

#### Proceso unificado

Modelo de proceso evolutivo y compuesto por cuatro fases:

- Inicio/Concepción
- Elaboración
- Construcción
- Transición

Es un modelo de proceso adaptable a la complejidad y tipo de sistema. Se centra en la arquitectura, mostrando y decidiendo los distintos aspectos arquitectónicos que presenta un sistema software de etapas tempranas que servirán de base a las futuras.

Se dirige por casos de uso, desarrollándose en cada iteración determinados casos de uso. Eligiendo para iteraciones tempranas los casos de uso que determinan la arquitectura

**Problema: ** (en general de los ciclos evolutivos) si dividimos en partes el sistema, a la hora de aunarlo puede dar problemas, no vemos el "todo"

![](/home/clara/.config/Typora/typora-user-images/image-20200224153627090.png)

![image-20200224154625039](/home/clara/.config/Typora/typora-user-images/image-20200224154625039.png)

Las acciones y tareas de cada fase son:

- **Inicio:** estudio de viabilidad, alcance, objetivos y planificación del proyecto, análisis de riesgos, determinación de los requisitos fundamentales del sistema y propuesta de una arquitectura determinada
- **Elaboración:** ajustes de la planificación del proyecto y desarrollo completo de la arquitectura básica sobre la que se asentará la fase de construcción
- **Construcción: **se completa los modelos de requisitos y diseño de la elaboración, se implementan los elementos necesarios para completar el sistema y se realizan las pruebas de los distintos elementos que se van terminando, se integran y se hacen pruebas de aceptación por parte de usuario
- **Transición: **asegurarse que el sistema cumple con los requisitos especificados (pruebas por los usuarios) y tareas relacionadas con el despliegue de la estructura general de proceso, para preparar lo necesario para su lanzamiento al mercado

###### Img. ejemplo concreto de PU para un sistema simple

![image-20200224155047086](/home/clara/.config/Typora/typora-user-images/image-20200224155047086.png)

#### Desarrollo ágil

> *¿Por qué tantos proyectos de desarrollo de software no se terminan a tiempo, cuestan más que lo presupuestado originalmente, tienen problemas de calidad serios y generan menor valor que el esperado?* Se preguntaron 17 expertos, que después elaboraron el Manifiesto Ágil

##### Características:

- Proceso iterativo e incremental (evolutivo)
- Entregas frecuentes
- Trabajo en equipo
- Autonomía del equipo de desarrollo
- Revisiones y reuniones retrospectivas frecuentes

##### Beneficios:

- Desarrollo guiado por valor 
- Mejor manejo de riesgos e incertidumbres 
- Mejora la productividad

##### Métodos y técnicas:

- SCRUM
- Extreme Programming
- Programación en parejas
- Test Driven Developement>