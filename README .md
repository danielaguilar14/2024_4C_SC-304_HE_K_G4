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







