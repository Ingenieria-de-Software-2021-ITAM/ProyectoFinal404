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

# 1. Introduction<a name="1"></a>

## 1.1 Purpose<a name="11"></a>

## 1.2 Document Conventions<a name="12"></a>

## 1.3 Intended Audience and Reading Suggestions<a name="13"></a>

## 1.4 Product Scope<a name="14"></a>

## 1.5 References<a name="15"></a>


# 2. Overall Description<a name="2"></a>

## 2.1 Product Perspective<a name="21"></a> 

## 2.2 Product Functions<a name="22"></a>

## 2.3 User Classes and Characteristics<a name="23"></a>

## 2.4 Operating Environment<a name="24"></a>

## 2.5 Design and Implementation Constraints<a name="25"></a>

## 2.6 User Documentation<a name="26"></a>

## 2.7 Assumptions and Dependencies<a name="27"></a> 

# 3. External Interface Requirements<a name="3"></a>

## 3.1 User Interfaces<a name="31"></a>

## 3.2 Hardware Interfaces<a name="32"></a>

## 3.3 Software Interfaces<a name="33"></a>

## 3.4 Communication Interfaces<a name="34"></a>

# 4. System Features<a name="4"></a>
## 4.1 Login<a name="41"></a>
Los alumnos del ITAM podrán ingresar a la página web usando las mismas credenciales que han usado siempre.
## 4.2 Subir propuestas<a name="42"></a>
Cualquier usuario podrá subir una propuesta sobre un proyecto a la plataforma. Esto lo hará *solamente* desde su propia cuenta.
## 4.3 Calificación a los proyectos<a name="43"></a>
Los usuarios podrán calificar las propuestas hechas por otros usuarios. Para hacerlo más interactivo y que la aplicación congenie mejor los estudiantes, la propuesta será evaluada en función de cuántos "colmillos" tiene; es decir, cada propuesta tendrá una calificación que va desde cero a cinco colmillos.
## 4.4 Comentarios<a name="44"></a>
Los usuarios podrán comentar las propuestas hechas por otros usuarios. Habrá comentarios anidados; es decir, un usuario podrá comentar el comentario de otro usuario y así sucesivamente. Los comentarios también serán calificados por los usuarios con la misma escala descrita en la sección anterior y serán mostrados según su calificación, con los comentarios mejor evaluados hasta arriba. Para que se puedan ordenar, se debe cumplir con un mínimo de evaluaciones.
## 4.5 Edición e historial de propuestas<a name="45"></a>
Los usuarios podrán editar sus propias propuestas ya publicadas. Por esta razón, el resto de los usuarios será capaz de ver el historial de la propuesta en cuestión y evaluar cada versión independiente.
## 4.6 Etiquetas<a name="46"></a>
Los usuarios podrán agregar etiquetas a las propuestas, tales como "deportiva", "cultura", "académica", etcétera. Esto facilitará la búsqueda y filtro de proyectos.
## 4.7 Sección de "trending"<a name="47"></a>
La página contará con una sección que tenga los proyectos que sean tendencia en el momento. Así los usuarios podrán estar al corriente con propuestas que hagan los otros usuarios.
## 4.8 Perfiles<a name="48"></a>
Cada usuario contará con un perfil público en el que se verán sus propuestas publicadas y comentarios hechos a propuestas.
## 4.9 Seguimiento de proyectos<a name="49"></a>
Los usuarios podrán "seguir" un proyecto que les haya agradado para ver posibles ediciones, el estatus del proyecto, nuevos comentarios, lo que se necesita hacer, etcétera. Se enviará una notificación a los usuarios cada vez que haya un cambio en alguno de los proyectos que siguen.
## 4.10 Aprobación de proyectos<a name="410"></a>
Los proyectos que sean subidos por los usuarios deben pasar por un proceso de aprobación realizado por las autoridades del ITAM antes de ser publicados. 
## 4.11 Ocultar proyectos<a name="411"></a>
Los usuarios podrán elegir la opción de ocultar de su vista principal los proyectos por los que ya hayan votado o que ya hayan visto y no les interese.

# 5. Nonfunctional Requirements<a name="5"></a>

## 5.1 Performance Requirements<a name="51"></a>

## 5.2 Safety Requirements<a name="52"></a>

## 5.3 Security Requirements<a name="53"></a>

## 5.4 Software Quality Attributes<a name="54"></a>

## 5.5 Business Rules<a name="55"></a>
