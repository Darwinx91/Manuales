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

## CLONACIÓN DEL REPOSITORIO

### Repositorio Administrador

:::info Enlace del repositorio
https://github.com/Sebastian170123/SPG_CT-FASE-FINAL.git
:::

---

### Pasos para clonar el repositorio

```bash
cd C:\MisProyectos
mkdir MisProyectos
cd MisProyectos
git clone https://github.com/Sebastian170123/SPG_CT-FASE-FINAL.git
cd SPG_CT-FASE-FINAL
code .
