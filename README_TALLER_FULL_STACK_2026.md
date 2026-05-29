# 🌐 Taller Full Stack 2026

## Aplicación Web: Frontend + Backend + MySQL

---

## 📌 Descripción del proyecto

Este proyecto corresponde a una aplicación web full stack desarrollada con tecnologías básicas de frontend, backend y base de datos.

La aplicación permite capturar información desde un formulario web, enviarla al servidor mediante JavaScript y almacenarla en una base de datos MySQL.

En este proyecto se integran los siguientes componentes:

* Frontend: interfaz visual creada con HTML, CSS y JavaScript.
* Backend: servidor desarrollado con Node.js y Express.
* Base de datos: almacenamiento de la información en MySQL.
* Comunicación: envío de datos mediante Fetch API en formato JSON.

---

## 🧱 Stack tecnológico

| Componente              | Tecnología             |
| ----------------------- | ---------------------- |
| Frontend                | HTML, CSS, JavaScript  |
| Backend                 | Node.js + Express      |
| Base de datos           | MySQL                  |
| Comunicación            | Fetch API, HTTP y JSON |
| Editor recomendado      | Visual Studio Code     |
| Servidor local frontend | Live Server            |

---

## 📁 Estructura del proyecto

```bash
TALLER_FULL_STACK_2026/
├── backend/
│   ├── package.json
│   ├── package-lock.json
│   ├── server.js
│   └── node_modules/
│
├── frontend/
│   ├── index.html
│   ├── contacto.html
│   ├── ayuda.html
│   ├── css/
│   ├── js/
│   ├── img/
│   └── video/
│
├── .gitignore
├── Documentacion.pdf
└── README.md
```

---

## ⚙️ Requisitos previos

Antes de ejecutar el proyecto, el estudiante debe tener instalado:

* Node.js
* npm
* MySQL
* MySQL Workbench
* Visual Studio Code
* Extensión Live Server
* Git

---

## 🔧 Instalación del proyecto

### 1. Clonar el repositorio

```bash
git clone https://github.com/USUARIO/TALLER_FULL_STACK_2026.git
```

Luego ingresar a la carpeta:

```bash
cd TALLER_FULL_STACK_2026
```

---

## 🖥️ Configuración y ejecución del backend

### 1. Ingresar al backend

```bash
cd backend
```

### 2. Instalar dependencias

```bash
npm install
```

### 3. Ejecutar servidor

```bash
node server.js
```

Debe aparecer:

```bash
Servidor en: http://localhost:3000
```

---

## 🗄️ Configuración de la base de datos

Ejecutar en MySQL:

```sql
CREATE DATABASE contactos_db;

USE contactos_db;

CREATE TABLE contactos (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nombre VARCHAR(100),
  correo VARCHAR(100),
  mensaje TEXT
);
```

---

## 🔌 Configuración de conexión MySQL

En el archivo:

```bash
backend/server.js
```

Configurar:

```javascript
const db = mysql.createConnection({
  host: "localhost",
  user: "root",
  password: "root",
  database: "contactos_db"
});
```

Modificar usuario y contraseña según la configuración local.

---

## 🎨 Ejecución del frontend

1. Abrir el proyecto en Visual Studio Code.
2. Ingresar a la carpeta frontend.
3. Abrir el archivo index.html.
4. Click derecho.
5. Seleccionar:

```text
Open with Live Server
```

---

## 🔄 Flujo de funcionamiento

```text
Formulario HTML
      ↓
JavaScript con Fetch API
      ↓
Backend con Node.js y Express
      ↓
Base de datos MySQL
      ↓
Respuesta al usuario
```

### Explicación

1. El usuario completa el formulario.
2. JavaScript captura los datos.
3. Fetch API envía la información al backend.
4. Node.js recibe los datos.
5. Express procesa la petición.
6. MySQL guarda la información.
7. El backend responde al frontend.

---

## 🧪 Prueba del proyecto

### 1. Ejecutar backend

```bash
node server.js
```

### 2. Abrir frontend con Live Server

### 3. Completar formulario

### 4. Enviar información

### 5. Verificar en MySQL

```sql
SELECT * FROM contactos;
```

---

## ⚠️ Problemas comunes

| Problema                | Solución                          |
| ----------------------- | --------------------------------- |
| Error de conexión MySQL | Revisar usuario y contraseña      |
| El servidor no inicia   | Verificar instalación de Node.js  |
| Puerto ocupado          | Cambiar puerto en server.js       |
| Error CORS              | Verificar configuración de cors() |
| No se guardan datos     | Revisar consulta SQL              |
| Frontend no conecta     | Revisar URL de fetch()            |
| node_modules en GitHub  | Verificar .gitignore              |

---

## 📌 Recomendaciones

* Ejecutar primero el backend.
* Verificar que MySQL esté activo.
* Revisar usuario y contraseña de MySQL.
* No subir node_modules a GitHub.
* Revisar consola del navegador y terminal cuando exista un error.
* Mantener organizada la estructura del proyecto.

---

## ✅ Resultado esperado

El estudiante debe poder:

* Ejecutar frontend con Live Server.
* Ejecutar backend con Node.js.
* Conectar backend con MySQL.
* Enviar datos desde un formulario.
* Guardar información en la base de datos.
* Consultar registros almacenados.

---

## 📚 Propósito académico

Este proyecto busca fortalecer conocimientos sobre:

* Desarrollo frontend.
* Desarrollo backend.
* Integración con bases de datos.
* Comunicación cliente-servidor.
* Flujo de datos en aplicaciones web.
* Organización de proyectos full stack.

---

## 🆕 Cambios realizados

Se realizaron mejoras visuales y funcionales en la aplicación TechZone, implementando un diseño moderno y responsive utilizando Bootstrap.

### Cambios principales

* Creación de una tienda tecnológica con interfaz moderna.
* Implementación de menú de navegación funcional.
* Desarrollo de página de ayuda con preguntas frecuentes.
* Desarrollo de página de contacto con formulario dinámico.
* Integración de tarjetas y componentes Bootstrap.
* Mejora de estilos visuales y experiencia de usuario.
* Organización de carpetas del proyecto.
* Actualización y conexión del repositorio en GitHub.

Además, se documentó completamente el proceso de instalación, configuración y ejecución del sistema para facilitar el uso del proyecto.
