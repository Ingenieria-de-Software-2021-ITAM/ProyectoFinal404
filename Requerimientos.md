# System Requirements Specifications #

**ITAM Proyectos**

Version `2.0` approved

Prepared by Equipo 404NotFound

Instituto Tecnológico Autónomo de México

26 de noviembre de 2021

## Table of contents
[Revision History](#revision-history)
1. [Introduction](#1)
	1. [Purpose](#11)
	1. [Document Conventions](#12)
	1. [Intended Audience and Reading Suggestions](#13)
	1. [Product Scope](#14)
	1. [References](#15)
2. [Overall Description](#2)
	1. [Product Perspective](#21)
	1. [Product Functions](#22)
	1. [User Classes and Characteristics](#23)
	1. [Operating Environment](#24)
	1. [Design and Implementation Constraints](#25)
	1. [User Documentation](#26)
	1. [Assumptions and Dependencies](#27)
3. [External Interface Requirements](#3)
	1. [User Interfaces](#31)
	1. [Hardware Interfaces](#32)
	1. [Software Interfaces](#33)
	1. [Communication Interfaces](#34)
4. [System Features](#4)
	1. [Login](#41)
	2. [Subir propuestas](#42)
	3. [Calificación a los proyectos](#43)
	4. [Comentarios](#44)
	5. [Edición e historial de propuestas](#45)
	6. [Etiquetas](#46)
	7. [Sección de "trending"](#47)
	8. [Perfiles](#48)
	9. [Seguimiento de proyectos](#49)
	10. [Aprobación de proyectos](#410)
	11. [Ocultar proyectos](#411)
5. [Nonfunctional Requirements](#5)
	1. [Performance Requirements](#51)
	1. [Safety Requirements](#52)
	1. [Security Requirements](#53)
	1. [Software Quality Attributes](#54)
	1. [Business Rules](#55)

## Revision History
| Name | Date | Reason for Changes | Version |
|----- | ----- | ----- |----- |
| Equipo 404NotFound | 19/11/2021 | Creación del documento entre todos | `1.0` |
| Equipo 404NotFound | 24/11/2021 | Implementación del documento que vimos en clase| `2.0` |

## 1. Introduction<a name="1"></a>

### 1.1 Purpose<a name="11"></a>
El presente proyecto tiene como motivación el desarrollo de una apliación web que permita a los alumnos, profesores y administrativos del ITAM enviar propuestas, que el resto de la comunidad las vea y que, por lo tanto, se facilite la implementación de dichas propuestas. El fin último es, pues, generar comunidad en beneficio de todos.

### 1.2 Document Conventions<a name="12"></a>
Para realizar este proyecto, nos hemos apegado a las formas que hemos visto a lo largo del curso de Ingeniería de Software. 

### 1.3 Intended Audience and Reading Suggestions<a name="13"></a>
Este documento está pensado principalmente para la maestra, quien evaluará el desempeño de nuestro equipo; sin embargo, cualquier persona con un interés en hacer una implementación real y funcional del proyecto encontrará valor tanto en este documento como en el resto de los que se han trabajado. Si el o la lectora tiene un poco de prisa, pero desea conocer con suficiente detalle la planeación de este proyecto y las funcionalidades que se implementan en él, entonces sugiero que vaya directamente a la sección de [System Features](#4). De cualquier manera, este documento se diseñó con la idea de no dar tantos rodeos.

### 1.4 Product Scope<a name="14"></a>
El software que se describe en este documento consiste en una página web en la que distintos miembros de la comunidad ITAM podrá manifestar sus ideas sobre proyectos que tenga en mente, darles forma, compartirlos, dar y recibir retroalimentación, perfeccionar su idea y, así, facilitar el proceso que se necesita para la implementación. Creemos que es un buen mecanismo para darle voz a estudiantes y otros miembros de la comunidad. 

### 1.5 References<a name="15"></a>
Como ya se mencionó, gran parte de la base de este proyecto, si no es que toda, está conformada por los temas cubiertos en la materia de Ingeniería de Software, impartido por la maestra Paulina Bustos Arellano. También queremos mencionar que el [prototipo](https://app.moqups.com/UOjb8TIzCNEXW9im5LEFTFgYHXaukQKI/view/page/aa1545f3c) de este proyecto se realizó utilizando la plataforma [moqups](https://moqups.com/es/).

## 2. Overall Description<a name="2"></a>

### 2.1 Product Perspective<a name="21"></a> 
Este producto será parte de la familia de páginas y servicios que ofrece el ITAM como universidad a su comunidad. Creemos que puede servir como extensión y soporte a los mecanismos que ya existen en el ITAM para dar forma a proyectos e ideas, como las representaciones de carreras u otras organizaciones estudiantiles. La aplicación se servirá a su vez de estos mismos servicios para obtener datos como correo electrónico, clave única, nombre, etcétera. 

### 2.2 Product Functions<a name="22"></a>
La funcionalidad principal de este producto es compartir propuestas de proyectos a otros usuarios y poder comentar, evaluar y refinar propuestas propias y ajenas.

### 2.3 User Classes and Characteristics<a name="23"></a>
El proyecto contará con dos tipos de usuarios: administradores y generales. Sus características se definen a continuación.
| Administradores | Generales |
|----- |----- |
| Tendrán la capacidad de revisar proyectos enviados antes de su publicación formal. Esto se hace con el fin de verificar que los proyectos cumplan con los lineamientos del reglamento y que no haya propuestas que no tienen lugar en nuestra institución. Al fungir como jueces, no podrán tomar parte en la evaluación de los proyectos ni podrán comentarlos. Su labor se limita a aprobar las propuestas. | Solamente podrán enviar propuestas, comentarlas y evaluarlas. No podrán dar autorización a proyectos de otros usuarios ni a los propios. |

### 2.4 Operating Environment<a name="24"></a>
La aplicación, como ya se mencionó, será una aplicación web. Funcionará con los navegadores más populares, como Chrome, Firefox, Safari y Edge. Para correr la aplicación, lo único que se necesita es acceso a un navegador y una conexión a internet activa. 

### 2.5 Design and Implementation Constraints<a name="25"></a>
Por temas de seguridad, como deseamos implementar el Login con credenciales del ITAM, los desarrolladores de este proyecto están limitados por las formas que el ITAM ya ha decidido que son seguras y confiables para poder ingresar en el sistema. Si bien el proceso no es el más atractivo y puede tener algunos obstáculos, creemos que es bastante seguro y vale la pena utilizarlo. También es cierto que la aplicación funcionará para computadora; habrá que adaptarla para celular más adelante. Fuera de eso, no debería ser una aplicación muy difícil de ejecutar ni que necesite equipo tan especial.

### 2.6 User Documentation<a name="26"></a>
Se pueden encontrar fácilmente la [documentación para replicar el proyecto](https://github.com/Ingenieria-de-Software-2021-ITAM/ProyectoFinal404/blob/main/DocumentacionReplicar.md) y un [diagrama de caso de uso](https://github.com/Ingenieria-de-Software-2021-ITAM/ProyectoFinal404/blob/main/DiagramaCasoDeUso.pdf). También se pone a disposición del usuario el [prototipo](https://app.moqups.com/UOjb8TIzCNEXW9im5LEFTFgYHXaukQKI/view/page/aa1545f3c) que hemos preparado para este proyecto.

### 2.7 Assumptions and Dependencies<a name="27"></a>
Estamos suponiendo —una gran suposición— que el ITAM nos permitirá utilizar los datos de los alumnos, así como que nos dará permiso de que los alumnos usen las mismas credenciales para entrar al sistema.

## 3. External Interface Requirements<a name="3"></a>

### 3.1 User Interfaces<a name="31"></a>
La interfaz de usuario, como ya se mencionó anteriormente, se modeló haciendo un [prototipo](https://app.moqups.com/UOjb8TIzCNEXW9im5LEFTFgYHXaukQKI/view/page/aa1545f3c) en la plataforma moqups. En el link proporcionado se puede consultar todo lo que concierne a este tema.

### 3.2 Hardware Interfaces<a name="32"></a>
Al tratarse de una página web, la interacción con el hardware está limitada a lo que comúnmente hacen las páginas web. No se requiere un hardware muy específico para poder navegar en internet; consecuentemente, tampoco hay muchos requerimientos de hardware para la página web.

### 3.3 Software Interfaces<a name="33"></a>
La aplicación tendrá interacción con una base de datos central en la que estarán registradastodas las propuestas, así como sus comentarios, evaluaciones, etcétera. También es necesario que la aplicación sea capaz de interactuar con la base de datos del ITAM en la que se almacenan los nombres de usuarios y contraseñas. Si no puede acceder directamente a ella, que por lo menos sea a través de una herramienta, de una manera análoga a lo que sucede con la aplicación Canvas.

### 3.4 Communication Interfaces<a name="34"></a>
Las notificaciones se enviarán por medio de correo electrónico, por lo que hay que tomar en cuenta la tecnología para comunicarse por este medio. También será necesario que la aplicación funcione mediante una conexión segura y un protocolo conocido, como lo es `https`. La transferencia de datos desde la base de datos del ITAM a la verificación de nuestro sitio web debe ser lo más segura y eficiente posible.

## 4. System Features<a name="4"></a>

### 4.1 Login<a name="41"></a>

Los alumnos del ITAM podrán ingresar a la página web usando las mismas credenciales que han usado siempre.

### 4.2 Subir propuestas<a name="42"></a>

Cualquier usuario podrá subir una propuesta sobre un proyecto a la plataforma. Esto lo hará *solamente* desde su propia cuenta.

### 4.3 Calificación a los proyectos<a name="43"></a>

Los usuarios podrán calificar las propuestas hechas por otros usuarios. Para hacerlo más interactivo y que la aplicación congenie mejor los estudiantes, la propuesta será evaluada en función de cuántos "colmillos" tiene; es decir, cada propuesta tendrá una calificación que va desde cero a cinco colmillos.

### 4.4 Comentarios<a name="44"></a>

Los usuarios podrán comentar las propuestas hechas por otros usuarios. Habrá comentarios anidados; es decir, un usuario podrá comentar el comentario de otro usuario y así sucesivamente. Los comentarios también serán calificados por los usuarios con la misma escala descrita en la sección anterior y serán mostrados según su calificación, con los comentarios mejor evaluados hasta arriba. Para que se puedan ordenar, se debe cumplir con un mínimo de evaluaciones.

### 4.5 Edición e historial de propuestas<a name="45"></a>

Los usuarios podrán editar sus propias propuestas ya publicadas. Por esta razón, el resto de los usuarios será capaz de ver el historial de la propuesta en cuestión y evaluar cada versión independiente.

### 4.6 Etiquetas<a name="46"></a>

Los usuarios podrán agregar etiquetas a las propuestas, tales como "deportiva", "cultura", "académica", etcétera. Esto facilitará la búsqueda y filtro de proyectos.

### 4.7 Sección de "trending"<a name="47"></a>

La página contará con una sección que tenga los proyectos que sean tendencia en el momento. Así los usuarios podrán estar al corriente con propuestas que hagan los otros usuarios.

### 4.8 Perfiles<a name="48"></a>

Cada usuario contará con un perfil público en el que se verán sus propuestas publicadas y comentarios hechos a propuestas.

### 4.9 Seguimiento de proyectos<a name="49"></a>

Los usuarios podrán "seguir" un proyecto que les haya agradado para ver posibles ediciones, el estatus del proyecto, nuevos comentarios, lo que se necesita hacer, etcétera. Se enviará una notificación a los usuarios cada vez que haya un cambio en alguno de los proyectos que siguen.

### 4.10 Aprobación de proyectos<a name="410"></a>

Los proyectos que sean subidos por los usuarios deben pasar por un proceso de aprobación realizado por las autoridades del ITAM antes de ser publicados. 

### 4.11 Ocultar proyectos<a name="411"></a>

Los usuarios podrán elegir la opción de ocultar de su vista principal los proyectos por los que ya hayan votado o que ya hayan visto y no les interese.

## 5. Nonfunctional Requirements<a name="5"></a>

### 5.1 Performance Requirements<a name="51"></a>
La aplicación no deberá preocuparse por manejar transacciones inmediatas y simultáneas; como se trata de publicaciones de proyectos, sin embargo, sí es importante que soporte grandes cantidades de información, sobre todo por el tema de los comentarios anidados. 

### 5.2 Safety Requirements<a name="52"></a>
Al tratarse de una página web con un objetivo muy específico, el uso de este producto implica un riesgo muy bajo a la integridad física del usuario en cuestión. Sin embargo, como en cualquier plataforma en la que se puede evaluar el contenido publicado por otros usuarios, hay que tener presente el posible impacto que pueda tener este tipo de aplicación en la salud mental y emocional de quienes la usen. 

### 5.3 Security Requirements<a name="53"></a>
Nuestra principal preocupación en lo que concierne a seguridad es que no se filtren los datos personales ni las credenciales de nuestros usuarios para que sea posible acceder al sistema del ITAM de manera segura. Un tema, además de éste, que hay que resolver, es cómo vamos a saber de quién fue la idea originalmente; de por sí, la propiedad intelectual es complicada. Entonces tenemos que ver cómo podemos hacerle para que no sea posible plagiar ideas y presentarlas como propias en nuestra plataforma.

### 5.4 Software Quality Attributes<a name="54"></a>
Será de suma importancia que la página sea responsiva, ya que no hay un único tamaño de pantallas de computadora. También, en la medida de lo posible, se intentará que la página siempre esté disponible y no se desconecte de la red constantemente. 

### 5.5 Business Rules<a name="55"></a>
Esta aplicación se tendrá que apegar al reglamento del ITAM y a lo que las autoridades de la institución decidan. Insistimos: es un complemento a otros mecanismos; no es el único método ni la única vía para proponer un cambio en el ITAM.
