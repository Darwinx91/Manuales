---
title: MANUAL DE INSTALACIÓN
sidebar_position: 1
---

# MANUAL DE INSTALACIÓN  
## APP-SPGCT  
### SISTEMA PARTICIPATIVO DE GARANTÍA COMUNITARIO Y TERRITORIAL

---

## 1. Créditos a los desarrolladores

La elaboración de la aplicación se divide en varias fases, asignadas a diferentes grupos
responsables de su desarrollo:

***Fase 1 y Fase 2:*** 

Estas etapas son responsabilidad de los equipos asignados al desarrollo
inicial de la aplicación desde su fase conceptual, cumpliendo con los lineamientos,
requerimientos funcionales y técnicos establecidos por el Departamento de Desarrollo
Productivo.

***Fase 3:*** 

Se lleva a cabo la depuración de errores y la validación integral del
funcionamiento del sistema, con el objetivo de asegurar su estabilidad, rendimiento y
operatividad antes del primer despliegue en producción

***Fase 4:*** 

Se lleva a cabo la revisión de la documentación, la identificación y corrección de
errores detectados durante dicho proceso, así como la implementación del proceso de
dockerización para facilitar la portabilidad y despliegue del sistema.
En cada fase se encuentran identificados los nombres de las personas responsables del
desarrollo de la aplicación, desde su concepción inicial hasta su despliegue final y
correcto funcionamiento.

***Fase 5:*** 

Se lleva acabo el proceso de pruebas QA de la apliacion para su correcto funcionamiento y facilidad de usu para los usuario y capacitaciones, y genereracion de la acta entrega recepcion a las entidades beneficiarias GAD CAYAMBE.

***Construcción Fase 2***

Andrés Moya | andres.moya@intsuperior.edu.ec | 0988091107

Jean De la Cruz | jean.delacruz@intsuperior.edu.ec | 0997431311

Lisbeth Esmeralda | lisbeth.esmeralda@intsuperio.edu.ec | 0994846279

Omar Sani | omarxdj4@gmail.com | 0959491061

***Construcción Fase 3***

Omar Sani | omarxdj4@gmail.com | 0959491061

Stalyn Fernandez | stalynfg5@gmail.com | 0968809537

Darwin Campues | darwincampues2908@gmail.com | 0986265270

Michael Garcia | mg8462654@gmail.com| 0988493858

***Construcción Fase 4***

Abigail Imbaquingo | abigailimbaquingo2211@gmail.com | 0997500499

Sebastián Anchundia | sebitas2034as@gmail.com | 0963962157

***Construcción Fase 5***

Stalyn Fernandez | stalynfg5@gmail.com | 0968809537

Darwin Campues | darwincampues2908@gmail.com | 0986265270

Michael Garcia | mg8462654@gmail.com| 0988493858

---

## 2. Introducción:
La aplicación SPGCT (Sistema de Participación y Gestión de Certificación Técnica) ha
sido desarrollada como una herramienta tecnológica clave para mejorar el proceso de
veedurías agroecológicas dentro del cantón Cayambe. Su objetivo principal es digitalizar
y optimizar la recolección, almacenamiento y análisis de evaluaciones realizadas en
campo, promoviendo la transparencia, sostenibilidad y eficiencia del sistema de
certificación participativa.
Este manual de instalación está dirigido a técnicos, desarrolladores y personal capacitado
que requiera implementar o desplegar la aplicación en entornos de prueba o producción.
A lo largo del documento se detallan los pasos necesarios para instalar la API, configurar
la base de datos, preparar el entorno del frontend y generar el APK móvil para su uso en
dispositivos Android.

---

## 3. REQUISITOS

***Paso para clonar desde el GitHub:***
### Copia la URL del repositorio:

➢Ve al repositorio en GitHub que deseas clonar.

➢ Haz clic en el botón "Code" (color verde).

➢ Copia la URL que aparece (por defecto es HTTPS)

### Abrir la terminal o línea de comandos:

➢ En Windows: puedes usar CMD, PowerShell o Git Bash.

➢ En macOS o Linux: abre la Terminal.

### Ir a la carpeta donde quieres clonar el proyecto:

➢ cd Ruta/De/Tu/Carpeta

### Clonar el repositorio:

➢ git clone

https://github.com/gadipmcsoftware/fullstack_spgct.git

### Entrar en la carpeta del proyecto:

➢ cd proyecto

Ya tienes el proyecto clonado en tu equipo y puedes comenzar a trabajar con él.

---

## 4. Requisitos Mínimos
### Para Computadora (Desarrollo e Instalación)


| Recurso | Requisito mínimo |
|--------|------------------|
| **Sistema operativo** | Windows 10 / macOS 11 / Ubuntu 20.04 |
| **Procesador** | Intel Core i5 (4 núcleos) o equivalente |
| **Memoria RAM** | 8 GB |
| **Espacio en disco** | 10 GB libres (para código, MongoDB y dependencias) |
| **Software requerido** | Visual Studio 2022, Visual Studio Code, MongoDB, Node.js, Android Studio, Git |


### Para Teléfono (Uso de la Aplicación SPGCT - APK)

| Recurso | Requisito mínimo |
|--------|------------------|
| **Sistema operativo** | Android 8.0 (Oreo) o superior |
| **Memoria RAM** | 2 GB |
| **Almacenamiento** | 150 MB libres (para la aplicación y datos) |

---

## 5. Instalación de la aplicación Web

➢ Abrir en el visual code la capeta APP-SPGCT

➢ En la terminal del visual o puedes acceder a la carpeta en el git bash.

➢ Debemos instalar las siguientes dependencias:


```bash
nvm install
nvm install 18.20.4
nvm use 18.20.4
npm install -g @quasar/cli
npm install
```

➢ Y por último para lanzar la aplicación debemos colocar:

```bash
quasar dev
```
➢ Debe aparecer de la siguiente manera, esto nos muestra que fue lanzada
correctamente la aplicación:

![quasardev](/img/quasar.png)

### Interfaz Web:

![fondo](/img/fondo.png)

## 6. Lanzar APIS (USUARIO, DATOS):
➢ Abrimos el visual 22 y seleccionamos el archivo con extensión .sln:

![fondo](/img/api.png)

➢ Después de abrir el archivo en visual 22, presionamos en el signo de play color
verde para prender la API de usuarios:

![fondo](/img/aapi.png)

➢ Vista de la API usuarios:

![fondo](/img/use.png)

➢ Realizar el mismo procedimiento con la API datos:

➢ Vista de la API datos:

![fondo](/img/datos.png)

## 7. Creación de la base de datos en el Mongo DB:

➢ Abrir MongoDB Compass

Inicia MongoDB Compass o accede a tu cliente GUI favorito de MongoDB.
Conéctate a tu servidor MongoDB (usualmente mongodb://localhost:27017 si es local).

➢ Crear una base de datos

Haz clic en el botón + junto a "Databases" o "Create Database".

Nombre de la base de datos: spgct

Nombre de la primera colección: por ejemplo, Users (puedes crear las demás después)

Presiona Create Database

➢ Agregar más colecciones

Entra a la base de datos spgct.

Haz clic en "Create Collection"

Nombre: productor

Repite el proceso:

Nombre: use

➢ (Opcional) Insertar documentos

Puedes insertar documentos manualmente en cada colección o importar desde archivos
JSON.

➢ Debe mirarse de la siguiente manera: 

![fondo](/img/mongo.png)

## 8. Generar APK móvil Android Studio:

➢ Debemos configurar las variables de entrono:

```bash
1. Configuracion previas para construir apk
2. Configurar variables de entorno del sistema
3. JAVA_HOME = C:\Program Files\Java\jdk-17
4. ANDROID_HOME = C:\Users\<Usuario>\AppData\Local\Android\Sdk
5. NOTA IMPORTANTE: el path de android_home, funciona si se realiozo una instalacion completa de android studio.
```

➢ En la terminal de visual code debemos mandar el siguiente comando para que se carguen
las librerías y poder generar el APK en el adriod studio:

```bash

yarn quasar build -m capacitor -T android

```

➢ Abrimos el mismo archivo que abrimos en el visual code:

➢ Buscamos la carpeta src-capacitor.

➢ Y abrimos el Android, en el Android studio:

![fondo](/img/apk.png)

➢ Vista del APK:

![fondo](/img/movi.png)

➢ Correo y contraseña general para el veedor:

```bash
desarrollo.productivo25@gmail.com
gadip2025
```

## 9. INSTALACION CON EL DOCKER 

Clonar el repositorio del proyecto desde GitHub

Para obtener una copia local del proyecto, es necesario clonar el repositorio desde
GitHub. Siga los siguientes pasos:

➢ Asegúrese de tener Git instalado en su sistema.

Si no lo tiene, descárguelo desde:

```bash
https://github.com/gadipmcsoftware/fullstack_spgct.git
```

➢ Abra la terminal o símbolo del sistema (CMD).

➢ Diríjase a la carpeta donde desea clonar el proyecto.


```bash
cd C:\MisProyectos
mkdir MisProyectos
cd MisProyectos
git clone https://github.com/gadipmcsoftware/fullstack_spgct.git
```

➢ Acceda a la carpeta del proyecto:

```bash
cd SPG_CT-FASE-FINAL
```

## 10. Ejecutar el proyecto con Docker

Una vez clonado el proyecto, siga estos pasos para ejecutarlo utilizando Docker:

➢ Asegúrese de tener Docker instalado.

Si no lo tiene, descárguelo desde:

https://www.docker.com/products/docker-desktop

➢ Desde la carpeta raíz del proyecto, ejecute el siguiente comando:

  Si existe un archivo docker-compose.yml:

cmd

docker-compose up --build

Este comando construirá y levantará los servicios definidos.

 Si solo hay un Dockerfile, utilice:

cmd

docker build -t spg_ct_final .

docker run -p 8080:8080 spg_ct_final

(Asegúrese de verificar el puerto usado por la aplicación.)

➢ Espere a que Docker inicialice todos los servicios.

➢ Abra el navegador y acceda a la dirección:

http://localhost:8080

(O el puerto especificado en el Dockerfile o Compose)

➢ Para detener el contenedor:

cmd

docker-compose down

o si usó docker run, presione Ctrl + C en la terminal.

## 11. Crear el usuario desde la Api para ingresar al sistema SPG-CT

Abrir el visual 22 y desplegar las APIs y dirigirse a la api ApiUserSPGCT
desplegada

➢ DESDE LA ApiUserSPGCT

![fondo](/img/autentificacion.png)

➢ NOS DIRIGIMOS AUTHETICATION 

![fondo](/img/post.png)

➢ GUITATE DE ESTO PARA CREAR LAS CREDENCIALES

➢ Y creamos las credenciales de forma manual 

![fondo](/img/contrasena.png)


## 12. PASOS PARA DSPLEGAR LA SPCGT
Recomendado el node 18.20.4 para el funcionamiento correcto

Pasos de forma local

1.- nvm install

2.- nvm install 18.20.4

3.- nvm use 18.20.4

4.- npm install -g @quasar/cli

5.- npm install

6.- quasar dev

Después de eso lo que vamos a hacer es crear el Dockerfile y el Docker-compose.yml para hacer los contenedores

➢ Dockerfile

➢ Comando para crear la Imagen

```bash
docker build -t spgct .
```

➢ Comando para desplegar el contenedor por el puerto 9000

Usa la imagen base de Node.js 18.20.4

FROM node:18.20.4

Establece el directorio de trabajo dentro del contenedor

WORKDIR /appSpgctDock

➢ Copia los archivos de configuración de tu proyecto al contenedor

COPY package*.json ./

COPY postcss.config.cjs ./

RUN npm config set fetch-retries 5

RUN npm config set fetch-retry-mintimeout 20000

RUN npm config set fetch-retry-maxtimeout 120000

➢ Instala las dependencias del proyecto

RUN npm install --location=global @quasar/cli

RUN npm install

RUN npm install uuid

➢ Copia el resto de los archivos de tu proyecto al contenedor

COPY . .

➢ Expone el puerto que usará la aplicación

EXPOSE 9000

➢ Comando para lanzar el proyecto

CMD ["quasar", "dev"]

➢ docker run -d -it -p 9000:9000/tcp spgct

Docker-compose.yml

version: '3.8'

services:

spgct:

build: .

image: spgct

ports:

- '9000:9000' # Mapea el puerto 9000 del host al 9000 del contenedor

volumes:

- .:/appSpgctDock

- /appSpgctDock/node_modules # Evita sobrescribir node_modules

environment:

- NODE_ENV=development

- MONGO_URL=mongodb://mongo:27017/spgctdb # Usa el nombre del

servicio "mongo"

- HOST=0.0.0.0 # ¡Importante! Permite conexiones externas

working_dir: /appSpgctDock

depends_on:

- mongo

➢ Opcional: Si la app se cierra inmediatamente, usa este comando para mantenerla activa

command: sh -c "npm install && quasar dev"

mongo:

image: mongo:latest

ports:

- '27017:27017' # Expone MongoDB (útil para debug, pero no necesario para la app)

volumes:

- mongo_data:/data/db # Persistencia de datos

environment:

- MONGO_INITDB_DATABASE=spgctdb

volumes:

mongo_data:

## 13. Tecnologías Usadas:

➢ Visual Studio Code: Visual studio code un gestor de código, lo utilizamos para
escribir el código de la app.

➢ Visual Studio 22: Visual studio 22 nos permite ingresar a las APIS que tengamos
para que el proyecto funcione.

➢ MongoDB: Mongo db es un motor de base de datos en donde se almacenarán los
datos recolectados de las veedurías.

➢ Android Studio: Android Estudio nos permite generar un APK que será
importante si queremos utilizar en dispositivos móviles.

➢ Docker Desktop: Docker Desktop nos permite aplicaciones en contenedores (por
ejemplo, servidores web, bases de datos, APIs).

## 14. Lenguajes de código:

➢ Vue: Visual Studio Code es un gestor de código que utilizamos para escribir el
código de la app.

➢ Type Script: Visual Studio 2022 nos permite integrar las APIs necesarias para el
funcionamiento del proyecto.

➢ Java Script: MongoDB es un motor de base de datos donde se almacenarán los
datos recolectados de las veedurías.

➢ HTML: Android Studio nos permite generar un APK, lo cual es importante si
queremos utilizar la aplicación en dispositivos móviles.

➢ Dockerfile/YAML: Archivos utilizados para definir la configuración de los
contenedores Docker (Dockerfile) y los servicios relacionados (dockercompose.yml), facilitando la automatización del despliegue del sistema.