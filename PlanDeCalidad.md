# Test plan 

1. [Test plan identifier](#1)
2. [References](#2)
3. [Introduction](#3)
4. [Test Items](#4)
5. [Software Risk Issues](#5)
6. [Features to be tested](#6)
7. [Features not to be tested](#7)
8. [Approach](#8)
9. [Item Pass/Fail Criteria](#9) 
10. [Suspension Criteria and Resumption Requirements](#10)
11. [Test Deliverables](#11)
12. [Remaining Test Tasks](#12) 
13. [Environmental Needs](#13)
14. [Staffing and Training Needs](#14)
15. [Responsibilities](#15)
16. [Schedule](#16)
17. [Planning Risks and Contingencies](#17)
18. [Approvals](#18)


# 1. Test plan identifier <a name="1"></a>
```plan_de_calidad_v0_1```

  Fecha: 26/11/2021
  
  Autores: equipo 404NotFound

# 2. References<a name="2"></a>
  * Requerimientos

# 3. Introduction<a name="3"></a>
Este documento es el Plan de Calidad para la aplicación para proponer proyectos al ITAM. En este plan se verá lo relacionado con los requerimientos, precisando en la funcionalidad en la que derivan y lo que va a hacer la aplicación. El principal objetivo del plan asegurarse de que el proyecto cumple con el nivel y detalle necesario para la buena funcionalidad de la aplicación.

# 4. Test Items<a name="4"></a>
Lo siguiente es una lista de las funcionalidades a probar:
  * Editor de Moqups, versión actual

# 5. Software Risk Issues<a name="5"></a>
Hay varias partes del proyecto que no están bajo el control de la aplicación, pero tienen un impacto directo en el proceso y también deben verificarse.
  * La base de datos del ITAM con sus usuarios y contraseñas
  * Los servidores del ITAM en donde funcionará dicha aplicación 
  * La participación de los alumnos en el proyecto

# 6. Features to be tested<a name="6"></a>
La siguiente lista es de las funcionalidades de la aplicación que se deben probar 
  * Subir un proyecto nuevo desde una cuenta de usuario, usando las etiquetas para identificar el proyecto
  * Que los usuarios puedan calificar las propuestas y que se muestre en cada proyecto el promedio de calificación
  * Que los usuarios puedan comentar los proyectos y que dichos comentarios se guarden correctamente
  * Al seguir un proyecto, este se guarda en los proyectos guardados del usuario
  * Los filtros para cada proyecto, es decir, que se muestren de acuerdo con sus etiquetas, calificación, guardados o no por el usuario, si son "trending", etc.

# 7. Features not to be tested<a name="7"></a>
La siguiente es una lista de las áreas que no se probaran específicamente. Es posible que estas funcionalidades sean probadas indirectamente al probar las demás.
  * Login con el login del ITAM
  * Que las propuestas sean editables
  * La sección de "trending"
  * El perfil del usuario
  * Proceso de aprobación de una propuesta de proyecto

# 8. Approach<a name="8"></a>
Se va a probar mediante librerías las funcionalidades relacionadas con los usuarios directamente involucrados, es decir, el ciclo de subir un proyecto con sus etiquetas, ver los proyectos publicados, la funcionalidad para calificar y comentar los proyectos publicados. Por otro lado, se probará manualmente que todo se registre de manera adecuada en la base de datos y que el servidor funcione de manera óptima. 

También vamos a probar manualmente la aprobación de la publicación de un proyecto. Esto es, se creará un perfil de usuario y otro de administrador en donde el administrador pueda ver las propuestas antes de publicarlas en el sitio y determinar si estas van de acuerdo con las reglas de convivencia. 

Por último, mediante encuestas de satisfacción, les preguntaremos a los usuarios y administradores qué les parece la aplicación y en caso de, si hay alguna retroalimentación.

# 9. Item Pass/Fail Criteria<a name="9"></a>
Se busca un criterio de aprobación estricto, en donde si las pruebas no son exitosas no se aprobarán para la versión final. Además, se debe completar en su totalidad las pruebas establecidas para que la aplicación pueda ser usada por el público. Se tendrá como margen, en dado caso de tener que liberar la aplicación antes por tiempo, que no haya falla en las funcionalidades estructurales y esenciales para que haya una operatividad que no entorpezca el uso de la aplicación.

# 10. Suspension Criteria and Resumption Requirements<a name="10"></a>

# 11. Test Deliverables<a name="11"></a>

# 12. Remaining Test Tasks<a name="12"></a>

# 13. Environmental Needs<a name="13"></a>

# 14. Staffing and Training Needs<a name="14"></a>

# 15. Responsibilities <a name="15"></a>

# 16. Schedule<a name="16"></a>

# 17. Planning Risks and Contingencies<a name="17"></a>

# 18. Approvals <a name="18"></a>
