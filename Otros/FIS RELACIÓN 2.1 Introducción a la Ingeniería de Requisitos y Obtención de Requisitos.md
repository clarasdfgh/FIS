# FIS RELACIÓN 2.1: Introducción a la Ingeniería de Requisitos y Obtención de Requisitos

### 1. Clasifique los siguientes requisitos, según su tipo:

- **FUNCIONALES**

  - Se llevará un control de todas los vehículos del establecimiento incluyendo su estado y disponibilidad

  - El conductor debe de poder dar al sistema las ordenes siguientes: Activar, Desactivar, Comenzar Aceleración, Parar Aceleración, y Continuar
  - Los usuarios podrán buscar, descargar e imprimir los artículos del repositorio de la biblioteca.

- **NO FUNCIONALES**

  - **Usabilidad**
    - A cada orden se le asignará un identificador único (ORDER-ID), que el usuario podrá copiar en el área de almacenamiento permanente de la cuenta
  - **Fiabilidad**
    - La aplicación estará disponible todos los días de la semana las 24 horas del día
    - La aplicación deberá poder reiniciarse y recuperar su funcionalidad al 100% antes de dos horas, tras producirse una caída por un fallo del tipo FA01
  - **Rendimiento**
  - **Soporte**
  - **Implementación**
    - Cada tipo de fichero tendrá asociado un programa de acceso en la aplicación
    - La interfaz de usuario deberá implementarse haciendo uso de html simple, sin marcos ni applets JAVA.
  - **Interfaz**
    - Sólo se levantará la barrera de entrada al aparcamiento tras haber reconocido la matrícula del vehículo situado ante la misma
  - **Operación**
    - Los usuarios deberán ser capaces de utilizar todas las funciones del programa tras recibir un curso de 3 horas de duración
  - **Empaquetamiento**
    - La aplicación funcionará sobre Windows 10
  - **Legales**
    - El proceso de desarrollo deberá ajustarse al estándar PSS-05 de ESA
    - El sistema no podrá mostrar a los operadores la información personal del cliente, salvo su nombre y número de referencia.

- **DE INFORMACIÓN:**

  - El producto debe llevar un registro de todas las carreteras que hayan sufrido daños
  - La aplicación deberá registrar los pagos de los recibos del impuesto del IBI

### 2. Proponga objetivos para una aplicación de apoyo a la docencia en la asignatura FIS

- Almacenar y gestionar la información relativa a cada alumno (información personal y privada de la asignatura, como notas) de forma que solo sea accesible al alumno y al problesor
- Informar a cada alumno dependiendo de su grupo y subgrupo de fechas de entregas próximas
- Tener una jerarquía de directorios accesible a los alumnos con los archivos necesarios tanto para teoría como para prácticas
- Consulta individual de cada alumno con todas las notas y entregas para el profesor

### 4. Considere el sistema de matriculación en la Universidad, enumere y clasifique los posibles implicados en la aplicación. Identifique posibles objetivos para los implicados de los distintos tipos. Identifique posibles áreas de conflicto entre los intereses de unos y otros

- **Alumnos**: usuario del sistema
  - Escoger asignatura
  - Escoger grupo
  - Escoger subgrupo
- **Profesores**: usuario del sistema
  - Registrar alumno en subgrupo
- **Administrativos**: usuario del producto
  - Registrar alumno en asignatura
  - Registrar alumno en grupo
  - Asignar profesor a grupo

Algunos conflictos existentes serían:

- Los alumnos querrían más facilidades para escoger grupo y asignaturas, por ejemplo con una lista de espera, pero esto alargaría los procesos burocráticos de los administrativos
- Los profesores querrían subgrupos menores para caber en las aulas pero conlleva más fragmentación de horarios a los alumnos

### 7. Realice un análisis y descripción de implicados para una aplicación de gestión de una biblioteca

- **Usuario:** persona sin carnet de biblioteca
  - Usuario del sistema
  - *Responsabilidades:*
    - Utilizar instalaciones
    - Consulta de material 
    - Sacarse carnet
  - *Criterios de éxito:*
    - El sistema le permite realizar sus actividades de la manera más sencilla posible
  - *Implicación:*
    - Puede utilizar todo lo disponible en la biblioteca menos las salas de estudio. No puede sacar material de la biblioteca. Puede sacarse el carnet de socio aportando un DNI
- **Socio:** persona con carnet de biblioteca o equivalente
  - Usuario del sistema
  - *Responsabilidades:*
    - Utilizar instalaciones
    - Consulta de material
    - Solicitar préstamo
    - Acceso a salas de estudio
  - *Criterios de éxito:*
    - El sistema le permite realizar sus actividades de la manera más sencilla posible.
  - *Implicación:*
    -  Tiene acceso a todas las actividades de la biblioteca porque tiene carnet: busqueda y consulta de material en la biblioteca, uso de salas de estudio y tomar material fuera de la biblioteca
- **Bibliotecario:** empleado de biblioteca
  - Usuario del producto
  - *Responsabilidades:*
    - Colocar libros
    - Navegar base de datos
    - Abrir salas de estudio
  - *Criterios de éxito:*
    - Hay éxito si en cualquier momento sabe donde colocar/encontrar cada libro, si no realiza préstamos inválidos (persona sin carnet, libro ya prestado...) y si no hay incompatibilidades en la gestión de las salas de estudio (misma aula a distintos solicitantes)
  - *Implicación:*
    - Son las personas de cara al público en la biblioteca, se encarga de orientar a las personas y colocar los libros según los usuarios los sacan
- **Bibliotecario jefe:** empleado y gestor de la biblioteca
  - Usuario del producto
  - *Responsabilidades:* 
    - Navegar base de datos
    - Gestionar base de datos
    - Dirigir bibliotecarios
    - Solicitar ejemplares
  - *Criterios de éxito:*
    - Tiene éxito si coordina y dirige correctamente a todos los bibliotecarios.
  - *Implicación:*
    - Conoce la base de datos en profundidad y dirige a cada bibliotecario para que ejerzan una función u otra
- **Administrador de la biblioteca:** administrativo encargado de la biblioteca
  - Usuario del producto
  - *Responsabilidades*
    - Navegar base de datos
    - Gestionar base de datos
    - Generar nueva base de datos
    - Contactar editorial
    - Gestionar presupuesto
    - Contratar gente
  - *Criterios de éxito:*
    - Tiene éxito si la base de datos es correcta y funciona bien para la biblioteca, si gestiona bien el presupuesto y tiene para conseguir nuevos libros de las editoriales
  - *Implicación:*
    - Administra el presupuesto y dirección de la biblioteca. Tiene que equilibrar los gastos de las instalaciones y los de ampliación de la oferta de la biblioteca. También decide el modelo de la base de datos

### 8. Realice una lista de objetivos y de requisitos estructurada de la gestión de una biblioteca

*OBJETIVOS:*

- **OBJ1.** Almacenar y gestionar de la base de datos de material (libros, películas, álbumes...)
- **OBJ2. **Almacenar y gestionar de la base de datos de los socios (préstamos presentes y pasados, amonestaciones...)
- **OBJ2.** Automatización de la gestión de préstamos asociados a cada usuario
- **OBJ3.** Gestión de los horarios y reservas de las salas de estudio

*REQUISITOS:*

- **RI1.** Base de datos de material
  - Tipo de material (libro, DVD, álbum...), ID, Título, Autor, Número total de préstamos, estado...
- **RI2.** Base de datos de los socios
  - DNI, Nombre y Apellidos, email, préstamos...



- **RF1.** Gestión de la base de datos de material
  - Control de la disponibilidad del material
  - Registrar o retirar material
  - Aceptar sugerencias
- **RF2.** Gestión de la base de datos de usuarios
  - Consulta de amonestaciones y de préstamos activos
  - Registrar, eliminar y modificar usuarios
- **RF3.** Préstamos
  - No prestar a usuarios sin carnet o con amonestaciones desatendidas
  - Mandar notificación previa a la amonestación al usuario
  - No procesar préstamos de libros agotados
- **RF4.** Salas de estudio
  - Registro con la hora de entrada y salida



- **RNF1. Usabilidad:** el sistema de búsqueda debe ser particularmente accesible, ya que está de cara al público y lo usará todo tipo de personas
- **RNF2. Fiabilidad:** se realizarán copias de seguridad periódicas de las bases de datos de material y usuarios, siendo más frecuentes las de material.
  - Se mantendrá, además, el sistema de clasificación con pegatinas en la contraportada del libro hasta que se adapte completamente la base de datos
- **RNF3. Empaquetamiento:** el sistema correrá en un ordenador con una distribución adaptada a la biblioteca de Ubuntu.
- **RNF4. Implementación:** se debe usar el lenguaje Java, compatible con Oracle Database para las bases de datos

 