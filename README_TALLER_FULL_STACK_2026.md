# 🌐 Taller Full Stack 2026

## Aplicación Web: Frontend + Backend + MySQL

---

# 📌 Descripción del proyecto

Este proyecto corresponde a una aplicación web full stack desarrollada con tecnologías básicas de frontend, backend y base de datos.

La aplicación permite capturar información desde un formulario web, enviarla al servidor mediante JavaScript y almacenarla en una base de datos MySQL.

El proyecto integra:

* Frontend desarrollado con HTML, CSS y JavaScript.
* Backend desarrollado con Node.js y Express.
* Base de datos MySQL.
* Comunicación mediante Fetch API usando JSON.

Además, se implementó una tienda tecnológica llamada **TechZone Store**, incluyendo páginas de inicio, ayuda y contacto con diseño responsive utilizando Bootstrap.

---

# 🧱 Stack tecnológico

| Componente         | Tecnología            |
| ------------------ | --------------------- |
| Frontend           | HTML, CSS, JavaScript |
| Backend            | Node.js + Express     |
| Base de datos      | MySQL                 |
| Comunicación       | Fetch API y JSON      |
| Framework CSS      | Bootstrap 5           |
| Editor recomendado | Visual Studio Code    |
| Servidor local     | Live Server           |

---

# 📁 Estructura del proyecto

```bash
TALLER_FULL_STACK_2026/
│
├── .vscode/
│
├── backend/
│   ├── package-lock.json
│   ├── package.json
│   └── server.js
│
├── frontend/
│   ├── css/
│   │   └── estilos.css
│   │
│   ├── img/
│   │   └── logo_sena.png
│   │
│   ├── js/
│   │   └── script.js
│   │
│   ├── video/
│   │   └── video_guille.mp4
│   │
│   ├── ayuda.html
│   ├── contacto.html
│   └── index.html
│
├── .gitattributes
├── .gitignore
├── Documentacion.pdf
└── README_TALLER_FULL_STACK_2026.md
```

---

# 📌 Descripción de carpetas

## 📂 backend

Contiene toda la lógica del servidor desarrollada con Node.js y Express.

### Archivos principales

* `server.js`: servidor principal y conexión con MySQL.
* `package.json`: configuración y dependencias.
* `package-lock.json`: control de dependencias instaladas.

---

## 📂 frontend

Contiene toda la interfaz gráfica de la aplicación web.

### 📂 css

* `estilos.css`: estilos personalizados del sitio.

### 📂 img

* `logo_sena.png`: imagen utilizada dentro del proyecto.

### 📂 js

* `script.js`: lógica JavaScript y conexión con el backend.

### 📂 video

* `video_guille.mp4`: archivo multimedia utilizado en el sitio.

### 📄 Archivos HTML

* `index.html`: página principal de TechZone Store.
* `ayuda.html`: centro de ayuda y preguntas frecuentes.
* `contacto.html`: formulario de contacto y atención.

---

# ⚙️ Requisitos previos

Antes de ejecutar el proyecto se debe tener instalado:

* Node.js
* npm
* MySQL
* MySQL Workbench
* Visual Studio Code
* Extensión Live Server
* Git

---

# 🔧 Instalación del proyecto

## 1. Clonar el repositorio

```bash
git clone https://github.com/USUARIO/TALLER_FULL_STACK_2026.git
```

## 2. Ingresar a la carpeta

```bash
cd TALLER_FULL_STACK_2026
```

---

# 🖥️ Configuración y ejecución del backend

## 1. Ingresar a la carpeta backend

```bash
cd backend
```

## 2. Instalar dependencias

```bash
npm install
```

## 3. Ejecutar servidor

```bash
node server.js
```

Si todo funciona correctamente aparecerá:

```bash
Servidor en: http://localhost:3000
```

---

# 🗄️ Configuración de la base de datos

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

# 🔌 Configuración de conexión MySQL

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

Modificar usuario y contraseña según la configuración local del computador.

---

# 🎨 Ejecución del frontend

## Pasos

1. Abrir el proyecto en Visual Studio Code.
2. Entrar a la carpeta `frontend`.
3. Abrir el archivo `index.html`.
4. Hacer clic derecho.
5. Seleccionar:

```text
Open with Live Server
```

El navegador abrirá automáticamente el sitio web.

---

# 🔄 Flujo de funcionamiento

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

---

# 🧪 Prueba del proyecto

## 1. Ejecutar backend

```bash
node server.js
```

## 2. Abrir frontend con Live Server

## 3. Completar formulario de contacto

## 4. Enviar datos

## 5. Verificar información en MySQL

```sql
SELECT * FROM contactos;
```

Si aparecen registros, la conexión funciona correctamente.

---

# ⚠️ Problemas comunes

| Problema                | Posible solución                    |
| ----------------------- | ----------------------------------- |
| Error de conexión MySQL | Revisar usuario y contraseña        |
| El servidor no inicia   | Verificar instalación de Node.js    |
| Puerto ocupado          | Cambiar puerto en `server.js`       |
| Error CORS              | Verificar configuración de `cors()` |
| No se guardan datos     | Revisar consulta SQL                |
| Frontend no conecta     | Revisar URL del fetch               |
| node_modules en GitHub  | Revisar `.gitignore`                |

---

# 📌 Recomendaciones

* Ejecutar primero el backend.
* Verificar que MySQL esté activo.
* Revisar usuario y contraseña de MySQL.
* No subir `node_modules` a GitHub.
* Revisar consola y terminal cuando exista un error.
* Mantener organizada la estructura del proyecto.

---

# ✅ Resultado esperado

El estudiante debe poder:

* Ejecutar frontend con Live Server.
* Ejecutar backend con Node.js.
* Conectar backend con MySQL.
* Enviar datos desde formularios HTML.
* Guardar datos en la base de datos.
* Consultar registros almacenados.

---

# 🎨 Cambios realizados

Se realizaron mejoras visuales y funcionales en la aplicación web TechZone Store.

## Mejoras implementadas

* Diseño moderno y responsive utilizando Bootstrap 5.
* Creación de una tienda tecnológica interactiva.
* Implementación de barra de navegación funcional.
* Desarrollo de página de ayuda con acordeones y preguntas frecuentes.
* Desarrollo de página de contacto con formulario dinámico.
* Integración de tarjetas informativas y efectos visuales.
* Mejora de experiencia de usuario y organización visual.
* Conexión del frontend con backend y MySQL.
* Actualización del repositorio en GitHub.

---

# 📚 Propósito académico

Este taller tiene como propósito fortalecer conocimientos relacionados con:

* Desarrollo frontend.
* Desarrollo backend.
* Bases de datos MySQL.
* Comunicación cliente-servidor.
* Integración full stack.
* Organización de proyectos web.
* Uso de Git y GitHub.
* Flujo de datos en aplicaciones web.

