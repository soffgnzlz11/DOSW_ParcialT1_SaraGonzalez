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



