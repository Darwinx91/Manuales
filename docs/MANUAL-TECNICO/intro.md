---
title: MANUAL TÉCNICO
sidebar_position: 1
---

# MANUAL TÉCNICO  
## APP-SPGCT  
### SISTEMA PARTICIPATIVO DE GARANTÍA COMUNITARIO TERRITORIAL

---

## 1. INTRODUCCIÓN

El presente **Manual Técnico** tiene como objetivo proporcionar información detallada sobre la **instalación, configuración y funcionamiento** de la aplicación **APP-SPGCT**, dirigida principalmente a:

- Desarrolladores  
- Administradores del sistema  
- Personal técnico  

Este documento sirve como una **guía de referencia técnica**, orientada a garantizar la correcta **implementación, mantenimiento y resolución de problemas** relacionados con la aplicación.

La información aquí presentada permite comprender la estructura del sistema, su propósito y los componentes que lo conforman, facilitando su análisis y soporte técnico en entornos académicos y profesionales.

---

## 2. DEFINICIONES

### SISTEMA PARTICIPATIVO DE GARANTÍA COMUNITARIO TERRITORIAL (SPG-CT)

La aplicación **APP-SPGCT** es una herramienta tecnológica diseñada para facilitar el **levantamiento de datos**, el **seguimiento** y la **gestión eficiente de veedurías** de productores agroecológicos en el cantón **Cayambe**, así como el **análisis de la información** obtenida en cada proceso de evaluación.

Permite centralizar la información recolectada durante las veedurías y apoyar la toma de decisiones mediante plataformas digitales.

---

### CARACTERÍSTICAS PRINCIPALES DEL SISTEMA

Entre las principales características del sistema **APP-SPGCT** se destacan:

#### • Manejo de usuarios
El sistema dispone de distintos **perfiles de usuario**, permitiendo controlar el acceso y las funcionalidades según el rol asignado.

#### • Registro de veedurías
La aplicación cuenta con una interfaz **intuitiva y amigable**, que permite registrar veedurías incluso **sin conexión a internet**, facilitando su uso en **zonas rurales o remotas**.

Las veedurías consideran las siguientes dimensiones:

- Áreas de interés  
- Dimensión política  
- Dimensión socioeconómica  
- Dimensión cultural  
- Dimensión económica  
- Dimensión ecológica  

#### • Gestión de reportes
Permite la **generación y almacenamiento de reportes**, incluyendo:

- Áreas de mejora  
- Irregularidades detectadas  
- Resultados del proceso de evaluación  

---

### ENFOQUE DEL SISTEMA

La aplicación **APP-SPGCT** prioriza la **accesibilidad** y la **usabilidad**, promoviendo la participación ciudadana y fortaleciendo la democracia local.

Sus objetivos principales son:

- Empoderar a la ciudadanía  
- Promover la rendición de cuentas  
- Apoyar una gestión pública responsable  
- Atender las necesidades reales de la comunidad  

---

## 3. PÚBLICO OBJETIVO

El público objetivo del sistema **APP-SPGCT** se divide según los roles definidos dentro de la aplicación.

---

### 3.1 VEEDORES

Los **veedores** garantizan la transparencia y credibilidad del proceso de certificación dentro del **SPG-CT**.

#### 3.1.1 FUNCIONES PRINCIPALES

- **Verificación en campo**  
  Registro de observaciones, fotografías y notas técnicas.

- **Monitoreo de cumplimiento**  
  Validación de estándares agroecológicos vigentes.

---

### 3.2 DEPARTAMENTO DE DESARROLLO PRODUCTIVO

Entidad encargada de supervisar y fortalecer el desarrollo agrícola sostenible del territorio.

#### 3.2.1 OBJETIVOS PRINCIPALES

- Fomentar la producción agroecológica  
- Brindar soporte técnico  
- Promover buenas prácticas agrícolas  

#### 3.2.2 HERRAMIENTAS EN LA APLICACIÓN

- **Panel de análisis**  
- **Gestión de solicitudes**  
- **Canales de comunicación**  

---

## 4. TECNOLOGÍAS UTILIZADAS

---

### 4.1 FRONTEND

- **Framework:** Vue.js + Quasar  
- **Lenguaje:** TypeScript  
- **Gestión de estado:** Pinia  
- **Consumo de APIs:** Axios  
- **Construcción APK:** Gradle  
- **Contenedores:** Docker  

---

### 4.2 BACKEND

- **Lenguaje:** C#  
- **Framework:** .NET 8  
- **Seguridad:** API de autenticación  
- **Contenedores:** Docker  

---

### 4.3 BASE DE DATOS

- **Motor:** MongoDB  
- **Entorno:** Local  
- **Contenedores:** Docker  

---

### 4.4 HERRAMIENTAS DE DESARROLLO

- Visual Studio Code  
- Visual Studio 2022  
- Insomnia  
- Android Studio  
- Docker  

---

## 5. REQUERIMIENTOS MÍNIMOS

---

### 5.1 HARDWARE

**Desarrollo:**

- Procesador Intel Core i3/i5 o superior  
- 8 GB RAM  
- 100 GB de espacio libre  

**Dispositivos móviles:**

- Android 5.0 o superior  
- 100 MB libres  

---

### 5.2 SOFTWARE

- Visual Studio Code  
- Visual Studio 2022 (.NET 8)  
- Insomnia  
- Android Studio  
- Node.js  

---

### 5.3 BASE DE DATOS

- MongoDB (local)

---

### 5.4 CONSTRUCCIÓN

- Gradle

---

### 5.5 CONTROL DE VERSIONES

- Git + GitHub

---

### 5.6 REPOSITORIOS DEL SISTEMA

- **SPGCT-Admin**  
- **SPGCT-Datos**  
- **SPGCT-Usuarios**

---

## 6. INSTALACIÓN DEL SISTEMA  
### APP-SPGCT – SPGCT-ADMIN  
### API-USUARIOS / API-DATOS

---

## 7. CLONACIÓN DEL REPOSITORIO

### Repositorio Administrador

:::info Enlace del repositorio
https://github.com/gadipmcsoftware/fullstack_spgct.git
:::

---

### Pasos para clonar el repositorio

```bash
cd C:\MisProyectos
mkdir MisProyectos
cd MisProyectos
git clone https://github.com/gadipmcsoftware/fullstack_spgct.git
cd SPG_CT-FASE-FINAL
code .
```
---
## 8. Instalación de NVM (Node Version Manager)

Descarga e instala **NVM** desde el sitio oficial.  
Si ya lo tienes instalado, no es necesario volver a instalarlo.

https://github.com/coreybutler/nvm-windows/releases

### Verificar la instalación

```bash
nvm --version
```
### Instalar Node.js
```bash
nvm install 18.20.4
```
### Activar la versión instalada
```bash
nvm use 18.20.4
```
### Confirmar la versión activa
```bash
node -v
```
---
## 9. Instalar el Cliente de Quasar
### Instalar Quasar CLI globalmente
```bash
npm install -g @quasar/cli
```
También puedes consultar el comando actualizado en la página oficial de Quasar.
### Verificar la instalación
```bash
quasar --version
```
### Si ocurre algún error ejecutar
```bash
npm install
```
---
## 10. Lanzar el Proyecto
### Ejecutar el proyecto
En la terminal, dentro del directorio del proyecto, ejecuta el siguiente comando para iniciar la aplicación:
```bash
quasar dev
```
### Acceder a la aplicación
Abre tu navegador y entra a la URL que aparece en la terminal, normalmente:
http://localhost:9000


Se mostraria en el puerto 9000 como se muestre en la imagen:

![Instalación de NVM](/img/fondo.png)
---
## 11. Instalación Backend
### Clonar el Repositorio
Abre una terminal o línea de comandos de git.
Ejecuta el siguiente comando para clonar los repositorios de la aplicación:
Para Api Usuarios y Api DATOS que se encuentra en el mismi github de toda la aplicacion.

:::info Enlace del repositorio
https://github.com/gadipmcsoftware/fullstack_spgct.git
:::

### Pasos para clonado de un repositorio:

```bash
cd C:\MisProyectos
mkdir MisProyectos
cd MisProyectos
git clone https://github.com/gadipmcsoftware/fullstack_spgct.git
cd SPG_CT-FASE-FINAL
code .
```
---
### Abre la aplicación Visual estudio 22

Lanza el proyecto en los diferentes entornos de Development , Testing o Production 
Roles de Usuarios:
### Introducción a los Roles de Usuario
En nuestra aplicación, se han definido distintos roles de usuario con permisos y accesos
específicos para garantizar una gestión eficiente y segura de la información. Los roles de
Desarrollo Productivo y Veedor han sido configurados con diferentes niveles de
interacción con la plataforma, basados en las necesidades y funciones de cada grupo.

| Módulo / Acción | Desarrollo Productivo (Accesos) | Veedor (Accesos) | Desarrollo Productivo (Interacción con App) | Veedor (Interacción con App) |
|-----------------|----------------------------------|------------------|---------------------------------------------|--------------------------------|
| **Registrar Usuario** | Departamento de Desarrollo de Software es el único que puede registrar y recuperar contraseñas según el modelo de la aplicación | - | - | - |
| **Añadir Productor** | Permitido | Permitido | Puede registrar productor | Puede registrar productor |
| **Productores** | Permitido | Denegado | Buscar, eliminar y subir datos a la base (registros, veedurías por tablet) | Denegado |
| **Dashboard** | Permitido | Denegado | Buscar y descargar registros en Excel | Denegado |
| **Historial** | Permitido | Permitido | Visualiza registros por tablet y los sube a la base con contraseña | Visualiza registros por tablet |
| **Resetear Password** | Permitido | Denegado | Cambio de contraseña | Denegado |
| **LocalStorage** | Agregado | Agregado | - | - |
| **Base de Datos y API** | Agregados | No | - | Registrar |

## 12 .Arquitectura y Funcionamiento de la Aplicación

### Interacción con Axios
En la aplicación se utiliza **Axios** para realizar solicitudes HTTP y comunicarse con las APIs del sistema.  
Se configuraron dos instancias principales:

- **api:** Conectada a la API principal para la gestión de datos generales.  
  URL base: `https://localhost:7026/api/`

- **apiUser:** Encargada del manejo de usuarios.  
  URL base: `https://localhost:7085/api/`

Ambas instancias se registran globalmente mediante la función **boot de Quasar**, lo que permite acceder a ellas desde cualquier componente sin necesidad de importarlas en cada archivo. Esto mejora la organización del código y centraliza la configuración de las APIs.

---

### Modelos de Datos
La aplicación utiliza **interfaces como modelos de datos** para estructurar y tipificar la información.

**UserModel**
Representa los datos de un usuario registrado:
- `id`: Identificador único del usuario.
- `name` y `lastName`: Nombre y apellido.
- `cedula`: Número de identificación.
- `email`: Correo electrónico del usuario.
- `password`: Contraseña para el acceso al sistema.

**ResetModel**
Se utiliza para gestionar la recuperación de contraseñas mediante correo electrónico:
- `recipientName`: Nombre del destinatario.
- `recipientEmail`: Correo electrónico del destinatario.
- `subject`: Asunto del mensaje.
- `body`: Contenido del correo.

El uso de modelos permite mantener consistencia en los datos, mejorar la legibilidad del código y reducir errores en la comunicación con la API y la base de datos.

---

### Registro de Usuarios
El registro permite a los nuevos usuarios ingresar sus datos mediante un formulario HTML en `indexPage.vue`.

Proceso general:
1. El usuario completa el formulario.
2. Los datos se enlazan mediante **v-model**.
3. Al enviar el formulario se ejecuta el método `register`.
4. Los datos se almacenan temporalmente en **localStorage**.
5. Posteriormente se envían a la API para su procesamiento.

Además, el sistema genera automáticamente una **contraseña segura** utilizando la clase `UserService`, la cual crea contraseñas con:
- Letras mayúsculas
- Letras minúsculas
- Números
- Longitud aproximada de 20 caracteres.

---

### Recuperación de Contraseña
El módulo de recuperación permite restablecer la contraseña usando el correo electrónico del usuario.

Flujo del proceso:
1. El usuario ingresa su correo en el formulario (`resetPassword.vue`).
2. Se valida el formato del correo.
3. El correo se almacena temporalmente en **localStorage**.
4. Se consulta en la base de datos si el usuario existe.
5. Si es válido, el backend genera una nueva contraseña y la envía al correo del usuario.

---

### Gestión del Estado con Pinia
La aplicación utiliza **Pinia** para manejar el estado global.

Mediante `defineStore` se crean **stores** que permiten:
- Gestionar datos compartidos entre componentes.
- Mantener la consistencia del estado de la aplicación.

Ejemplo:
El store `FormDimensionEcologica` gestiona las preguntas y respuestas del formulario de la dimensión ecológica, incluyendo el cálculo del **puntaje total**.

---

### Estructura de Formularios
Los formularios están construidos con **Vue.js y Quasar Framework**.

Características principales:
- Uso de `v-model` para enlace de datos.
- Eventos `@submit.prevent` para controlar el envío.
- Subformularios para registrar información adicional (por ejemplo, biofertilizantes).
- Funciones que realizan cálculos automáticos dentro de los formularios.

---

### Gestión de Productores
El módulo de productores permite consultar, registrar y gestionar datos de productores.

La función principal realiza:
- Solicitud **GET** a la API mediante Axios.
- Conversión de la respuesta a un arreglo de objetos `IProductorModel`.
- Manejo de errores mediante `try/catch`.

---

### Proceso de Autenticación (Login)
El proceso de autenticación sigue los siguientes pasos:

1. El usuario ingresa **correo y contraseña** en el formulario de login.
2. Las credenciales se almacenan temporalmente en **localStorage**.
3. Se envían a la API mediante una solicitud **POST**.
4. Si las credenciales son válidas, el servidor devuelve un **token de autenticación**.
5. El token se guarda en localStorage para mantener la sesión activa.
6. El usuario es redirigido al módulo correspondiente.

---

### Carga de Datos a la Base de Datos
El sistema permite registrar información de productores mediante la API.

Flujo:
1. Se recibe un objeto con los datos del productor.
2. Se convierte a formato **JSON**.
3. Se agrega el **token de autenticación** en los encabezados.
4. Se envía una solicitud **POST** al endpoint correspondiente de la API.

---

### Backend del Sistema
El backend está diseñado para manejar operaciones **CRUD** y gestionar usuarios.

Tecnologías principales:
- **Node.js**
- **MongoDB**
- **Mongoose** (ODM para la base de datos)
- **Nodemailer** para envío de correos electrónicos.

La API está documentada con **Swagger**, lo que permite visualizar los endpoints, parámetros y respuestas desde `/api-docs`.

---

### Seguridad del Sistema

#### Seguridad en el Frontend
La aplicación implementa control de acceso mediante **tokens de autenticación**.

Tipos de acceso:
- **Token local:** acceso limitado.
- **Token API:** acceso completo a funcionalidades.
- **Sin token:** acceso denegado.

Además:
- Las rutas se habilitan o bloquean dinámicamente.
- El menú lateral muestra solo las opciones permitidas.
- Existe una función para **cerrar sesión**, eliminando los tokens almacenados.

---

### Ejecución del Sistema con Docker
El sistema SPGCT también puede ejecutarse mediante contenedores Docker.

**Requisitos previos:**
- Docker Desktop instalado  
  https://www.docker.com/products/docker-desktop/

**Sistemas compatibles:**
- Windows 10 / 11 con WSL2
- Linux
- macOS
### Contenedores incluidos

Este sistema contiene los siguientes servicios:

![doker](/img/doker.png)
---
## 13. Acceso a la aplicación
Una vez los contenedores estén ejecutándose, se puede acceder a la aplicación desde el
navegador:

***Frontend (Quasar):***
- http://localhost:9000

***Backend (API):***
- http://localhost:8081/swagger/index.html
- http://localhost:8080/swagger/index.html

### Para detener los contenedores 
Desde la misma ruta, ejecutar: 

- bash 
 
•	Esto detendrá todos los servicios del sistema SPGCT. 
Verificar estado de los contenedores 


docker compose down:

• 	Para comprobar si los servicios están corriendo: 
 
docker ps 
 

