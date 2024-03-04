# 2024_4C_SC-304_HE_K_G4
Primer Avance del Proyecto de Investigación 
Profesor: 
MSc. José Andrés Alvarado Moreira
Integrantes del grupo #4:
Aguilar Aguilar Jose Daniel
Baltodano Obregón María José
Gomez Diaz Jose Daniel 
Fecha de entrega:
26-02-2024



- Plan de proyecto de investigación -
Desarrollo de plataforma de red social para la empresa el "Pajarito Feliz"

- Objetivo Principal del proyecto -
Desarrollar una plataforma de red social donde se permite a los ususarios compartir comentarios entre amigos con una relación directa.

- Tareas a realizar en la ejecución del proyecto -
1. Analisis de requisitos
   
   Se actegorizan en requisitos funcionales y no funcionales
   Responsable :
2. Diseño del sistema
   
   Definir la arquitectura del sistema.
   Diseñar la estructura del grafo
   Diseñar la estructura de la lista adyacente utilizando una Lista- Doble- Circular y una lista Simple.
   Responsable:
3. Implementación del backend
   
   Desarrollar las clases y métodos necesarios para la gestión de usuarios.
   Implementar la estructura de grafo utilizando la lista de adyacencia.
  Implementar la lógica para seguir a otros usuarios y validar su existencia.
   Desarrollar la gestión de mensajes utilizando una estructura de Pila.
  Responsable: 

4.. Implementación del frontend

  Diseñar e implementar la interfaz de usuario.
  Desarrollar la visualización de mensajes según las relaciones de seguimiento.
  Implementar la funcionalidad de agregar, editar y eliminar mensajes.
  Responsable:

5. Pruebas y depuración

  Realizar pruebas unitarias y de integración.
  Responsable:

6. Documentación

  Preparar documentación para usuarios finales.
  Documentar el código y los procesos de desarrollo.
  Responsable:

7. Administración de usuarios

  Desarrollar la funcionalidad de administración de usuarios para el administrador.
  Implementar la eliminación de usuarios y la eliminación de sus mensajes y relaciones de seguimiento.
  Responsable: 

   Primer Avance del Proyecto de Investigación

Profesor: MSc. José Andrés Alvarado Moreira 

Integrantes del grupo #4: 
Aguilar Aguilar Jose Daniel
Baltodano Obregón María José 
Gomez Diaz Jose Daniel

Fecha de entrega:
26-02-2024

● Plan de proyecto de investigación 
- Desarrollo de plataforma de red social para la empresa el "Pajarito Feliz"

Objetivo Principal del proyecto 
- Desarrollar una plataforma de red social donde se permita a los usuarios compartir comentarios entre amigos con una relación directa.

- Tareas a realizar en la ejecución del proyecto -

* Análisis de requisitos
  Se actegorizan en requisitos funcionales y no funcionales 
Encargado: Baltodano Obregón María José 

* Diseño del sistema
  Definir e identificar la arquitectura del sistema. 
  Diseñar la estructura del gráfico 
  Diseñar la estructura de la lista adyacente utilizando una Lista- Doble- Circular y una lista Simple. 
Encargado: Jose Daniel Gomez Diaz

* Implementación del backend
  Desarrollar las clases y métodos necesarios para la gestión de usuarios.
  Implementar la estructura de gráfico utilizando la lista de adyacencia.
  Implementar la lógica para seguir a otros usuarios y validar su existencia.
  Desarrollar la gestión de mensajes utilizando una estructura de Pila. 
Encargado: Jose Daniel Aguilar Aguilar

*Implementación del frontend
  Diseñar e implementar la interfaz de usuario. 
  Desarrollar la visualización de mensajes según las relaciones de seguimiento. 
  Implementar la funcionalidad de agregar, editar y eliminar mensajes. 
Encargado: Jose Daniel Aguilar Aguilar

*Pruebas y depuracion
  Realizar pruebas unitarias y de integración.
Encarargado:Jose Daniel Aguilar Aguilar

* Documentación
  Prepare documentación para usuarios finales. 
  Documentar el código y los procesos de desarrollo. 
Encargado: Baltodano Obregón María José

* Administración de usuarios
  Desarrollar la funcionalidad de administración de usuarios para el administrador. 
  Implementar la eliminación de usuarios y la eliminación de sus mensajes y relaciones de seguimiento. 
Encargado: Jose Daniel Gomez Diaz

CADA PERSONA SEGUN CLASE, Y LOS METODOS SEGUN EL DIAGRAMA.


﻿Clases Principales:
* Usuario:
   * Atributos Privados:
      * id: string
      * nombre: string
      * relaciones: ListaSimple
 *  Pila cada pila va a tener un arbol que tienedatos y cada(cada dato es un mensaje)
   * Métodos Públicos:
      * seguir(usuario: Usuario): void
      * publicarMensaje(mensaje: Mensaje): void
      * eliminarUsuario(): void
* Mensaje:
   * Atributos Privados:
      * id: string
      * contenido: string
      * fechaHora: Date
    
   * Métodos Públicos:
      * agregarRespuesta(respuesta: Mensaje): void ----> DENTRO DE USUARIO (PARAMETROS DE LO QUE RECIBE) QUE RECIBA UN OBJ MENJS DONDE SE SEPA QUIEN ES EL PADRE
-----> DENTRO DE CADA NODO PILA 
      * editarMensaje(nuevoContenido: string): void
      * eliminarMensaje(): void
* ListaDobleCircular: 
GRAFO sE CREA UNA CLASE GRAFO VA A TENER UNA LISTA CIRCULAR DOBLE 
SE TIENE QUE HACER UNA CLASE NODOGRAFO 



   * Atributos Privados:
      * primerNodo: NodoListaDobleCircular
   * Métodos Públicos:
      * agregarNodo(usuario: Usuario): void
      * eliminarNodo(usuario: Usuario): void
* NodoListaDobleCircular:
   * Atributos Privados:
      * usuario: Usuario
      * siguiente: NodoListaDobleCircular
      * anterior: NodoListaDobleCircular
* ArbolBinario:
UN ROOOT DE TIPO NODO ARBOL 
Y ESE NODO ARBOL TIENE UN OBJ DATO UN IZQ Y UN DERECHO 


   * Atributos Privados:
      * raiz: NodoArbolBinario
   * Métodos Públicos:
      * agregarNodo(respuesta: Mensaje): void
      * eliminarNodo(respuesta: Mensaje): void
* NodoArbolBinario:
   * Atributos Privados:
      * mensaje: Mensaje
      * izquierdo: NodoArbolBinario
      * derecho: NodoArbolBinario
Consideraciones:
* Estática o No Estática: Las clases representan instancias específicas y, por lo tanto, son no estáticas.
* Atributos Públicos y Privados: Se han definido algunos atributos como privados (private) para limitar el acceso directo, mientras que los métodos públicos permiten la interacción controlada con estos atributos.
* Git: Este diagrama de clases puede organizarse en un repositorio Git, preferiblemente en un archivo como "DiagramaDeClases.md" o similar.
Recuerda personalizar este esquema según las necesidades específicas y ajustes que puedan surgir durante el desarrollo del proyecto.




DISEÑO DE MENÚ E INTERFAZ DE USUARIO

Para diseñar una GUI se investigarán las posibles maneras de generarla programando con Java.
Para el diseño de esta GUI se tomará de referencia el diseño de la Red Social conocida como
Twitter o X.

Esta modalidad de interfaz de usuario es bastante simple y ha posibilitado enfocarse exclusivamente
en los aspectos relacionados con la programación orientada a objetos utilizando el lenguaje Java. No se ha 
tenido la necesidad de abordar simultáneamente la complejidad de trabajar con ventanas, botones y otros 
elementos similares.

Las interfaces gráficas de usuario (GUI) proporcionan al usuario ventanas, cuadros de diálogo, barras de
herramientas, botones, listas desplegables y diversos elementos con los que ya estamos familiarizados.
En este enfoque, las aplicaciones responden a eventos y se desarrollan haciendo uso de las clases
proporcionadas por la API de Java diseñadas específicamente para este propósito. Este cambio nos permite
crear aplicaciones más interactivas y amigables visualmente.

La estructura fundamental de la biblioteca se centra en componentes y contenedores. Los contenedores albergan 
componentes y, a su vez, son considerados componentes, permitiendo que los eventos sean manejados tanto en los
contenedores como en los propios componentes.

La API se compone de clases, interfaces y derivaciones, destacando las conocidas AWT y Swing como partes 
fundamentales de esta suite de herramientas para el desarrollo de interfaces gráficas en entornos Java.


Se utilizarán las siguientes clases con la siguiene jerarquía:

Component: superclase de todas las clases de interfaz gráfica.

Container: para agrupar componentes.

JComponent: superclase de todos los componentes de Swing
que se dibujan directamente en los lienzos (canvas).
Sus subclases son los elementos básicos de la GUI.

JFrame: ventana que no está contenida en otras ventanas.

JDialog: cuadro de diálogo.

JApplet: subclase de Applet para crear applets tipo Swing.

JPanel: contenedor invisible que mantiene componentes
de interfaz y que se puede anidar, colocándose en otros paneles
o en ventanas. También sirve de lienzo.

Graphics: clase abstracta que proporciona contextos gráficos
donde dibujar cadenas de texto, líneas y otras formas sencillas.

*****************************************************************
COMO SE VA ACOMPORTAR Y SUS SUB MENUS 
MENU PRINCIPAL AGREGAR ---> EXPLICAR QUE OPCIONES EL MENU VA ATENER,
1. AGREAR USUARIO (me pide datos del usuario y de una vez pedir a quien quiere seguir en una lista) (nuevo nodo en la lista)
2. ELIMINAR
3. ELIMINAR SEGUIMIENTOS 
4. VER FEET DE CUAL USUARIO?
5. ELIMINAR SEGUIMIENTO 
***************************************************************


TENER EL CODIGO DE LOS TEMAS QUE YA VIMOS EN CLASES 
TAREAS, CLASES,  MENU.




﻿Para desarrollar este proyecto, se pueden considerar el uso de las siguientes librerías y componentes visuales:


1. Frontend:


ReactJS: Para construir la interfaz de usuario y gestionar la lógica de la aplicación de manera eficiente.
Redux: Para gestionar el estado de la aplicación de manera centralizada.
React Router: Para manejar la navegación entre diferentes vistas de la aplicación.
Material-UI o Ant Design: Librerías de componentes visuales que facilitan la creación de interfaces atractivas y responsivas.


2. Backend:
Node.js y Express: Para construir el servidor que manejará las solicitudes y la lógica del negocio.
GraphQL (con Apollo Server): Para gestionar las consultas y mutaciones de manera eficiente.
Base de datos NoSQL (por ejemplo, MongoDB): Para almacenar la información de usuarios, relaciones, mensajes y comentarios.


3. Grafo y Estructura de Datos:


D3.js: Para visualizar el grafo de relaciones entre usuarios.
Lista-Doble-Circular y Lista-Simple: Puedes implementar estas estructuras de datos utilizando las capacidades de JavaScript, o incluso considerar librerías como Immutable.js si es necesario.


4. Mensajes y Comentarios:
Textarea o Input Component: Para permitir a los usuarios escribir mensajes y comentarios.
Moment.js: Para formatear y gestionar fechas y horas.
React Markdown: Si deseas permitir que los usuarios escriban mensajes con formato Markdown.


5. Árbol Binario para Respuestas:
Puedes implementar la estructura de un árbol binario utilizando las capacidades de JavaScript.


6. Seguridad:
JWT (JSON Web Tokens): Para gestionar la autenticación y autorización de usuarios.

Edición y Eliminación de Mensajes:
Se pueden implementar funcionalidades de edición y eliminación de mensajes utilizando lógica en el servidor y actualizando la interfaz de usuario correspondiente.


8. Eliminación de Usuario:
Utiliza algoritmos adecuados para recorrer y eliminar nodos en el árbol binario al eliminar un usuario.
