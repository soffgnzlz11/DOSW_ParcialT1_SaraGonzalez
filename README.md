# DOSW_ParcialT1_SaraGonzalez
## Parte 1 Diagrama de contexto - Analisis Inicial
<img width="901" height="694" alt="image" src="https://github.com/user-attachments/assets/8ccad877-03f6-4fd8-b359-68b33291a78f" />

## Parte 2 Requerimientos
# Diagramas de caso de Uso

### Historias de Usuario - HU-1

COMO estudiante de pregrado, QUIERO solicitar una tutoría con un Tutor - Profesor, PARA que el sistema me asigne el proximo tutor disponible.  
<img width="562" height="226" alt="image" src="https://github.com/user-attachments/assets/264f34a4-48f2-426a-acff-3eaca83224d9" />


### Historias de Usuario - HU-2
El sistema debe enviar una notificación una vez la reserva sea asugnada y confirmada.
COMO estudiante de pregrado, QUIERO solicitar una tutoría con un Tutor - Estudiante, PARA que el sistema me asigne el tutor disponible demi mismo programa.  
<img width="579" height="298" alt="image" src="https://github.com/user-attachments/assets/f5c4a527-4e9a-4069-9bca-e59da5c95311" />


### 📄 Requerimientos del Sistema

## 1. Lista general de requerimientos

El sistema TutoEci tiene los siguientes requerimientos para mejorar la experiencia académica implementando una plataforma para la gestión y asignación de tutorías.

### 1.1 Requerimientos funcionales

El sistema de Bankify debe tener la capacidad de:

1. El sistema TutoECI debe permitir a un Solicitantes (Estudiantes de Pregrado) solicitar una tutoria con un Tutor - Profesor.
2. El sistema TutoECI debe permitir a un Solicitantes (Estudiantes de Pregrado) solicitar una tutoria con un Tutor - Estudiante.
3. El sistema debe reservar a los Tutores-Profesores por 30 minutos.

### 1.2 Requerimientos no funcionales

El sistema de Bankify debe tener:

1. El sistema debe incorporar la paleta de colores oficial del programa de Ingeniería de Sistemas de la Escuela.
2. El sistema debe emplear una tipografía legible que cumpla con los estándares mínimos de contraste y accesibilidad web (WCAG 2.1 Nivel AA).

### Jira
https://dosw2026-2.atlassian.net/jira/software/projects/PSGT1/boards/4/backlog?selectedIssue=PSGT1-8
# 📄 Planeación del Sistema

### 1. Épica:

| Campo | Descripción |
|------|-------------|
| **ID** | EP-01 |
| **Título** |  Recomendación de Tutor  |
| **Descripción** | TechCup nesecita esta epica para permitir que el solicitante indique su preferencia de tutor y asi el Sistema le asigne el major tutor disponible. |
| **Stakeholder** | Sistema para brindar coleccion de tuores |
<img width="313" height="161" alt="image" src="https://github.com/user-attachments/assets/724cebdc-dfe3-4e60-932e-afdddabcb925" />


### 2. Historias de usuario:

| Campo | Descripción |
|------|-------------|
| **ID** | HU-01 |
| **Título** | Solicitar tutorial |
| **Descripción** | Como estudiante de pregrado, quiero solicitar una tutoría indicando mi preferencia de tutor 
(profesor o estudiante de posgrado), para que el sistema me asigne el mejor tutor disponible. |
| **Prioridad** |*[Media]* El Sistema debe seleccionar un tutor segun la preferencia del solicitante. |
| **Estimación** | *6* |

<img width="543" height="518" alt="image" src="https://github.com/user-attachments/assets/ac9fb3f5-b5af-4f04-a298-7191503e5e9d" />



### 3. Tareas:

| Campo | Descripción |
|------|-------------|
| **ID** | TR-01 |
| **Título** | Conectar a Enlace|
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Desarrollar la validacion de las materias del estudiante con su ID para mostrar los tutores disponibles.  |
| **Tareas requisito** | ninguna |
<img width="565" height="498" alt="image" src="https://github.com/user-attachments/assets/d70b1e30-9644-4877-86c9-1c71584414c4" />


| Campo | Descripción |
|------|-------------|
| **ID** | TR-02 |
| **Título** | Implementar creacion de solicitud (backend) |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Desarrollar el endpoint y la logica para registrar la solicitud en el sistema. |
| **Tareas requisito** | TR-01 |
<img width="513" height="522" alt="image" src="https://github.com/user-attachments/assets/3f7e92f9-351b-4403-887e-9c939ec71118" />


| Campo | Descripción |
|------|-------------|
| **ID** | TR-03 |
| **Título** | Implementar preferencias |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Desarrollar la recepcion de preferencias del estudiante para asignarle el mejor tutor. |
| **Tareas requisito** | TR-01 |
<img width="536" height="494" alt="image" src="https://github.com/user-attachments/assets/ebd30591-030e-494c-be18-4eeacc093356" />




### Ultimo Punto Patrones de diseño
## Diseño de Software y Patrones 
Identifique 2 patrones de diseño aplicables a este caso de estudio (por ejemplo, uno para 
la estrategia de selección de preferencia y otro para aislar la interoperabilidad con los 
sistemas externos). Especifique: 
• Nombre del patrón. 
• Tipo de patrón (creacional, estructural o de comportamiento). 
• Justificación de la decisión.  

## Patron Estructural Adapter 
Adapter es un patrón de diseño estructural que permite la colaboración entre objetos con interfaces incompatibles.
Podemos ver este patron reflejado en la historia de usuario donde el solicitante requiere de una tutoria entonces el sistema debe colaborar con enlace para obtener todos sus datos.

## Patron de diseño Singleton
Singleton es un patrón de diseño creacional que permite asegurse de que una clase tenga una única instancia.
Este patron se ve reflejado cuando se crean las diferentes clases de preferencia que se ha creado un objeto y al cabo de un tiempo creamos otro nuevo. En lugar de recibir un objeto nuevo, obtenemos lo que ya habíamos creado en las clases de preferencia.



