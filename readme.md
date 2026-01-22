# 🗃️ 1790 - Introducción a SQL con MySQL

<div align="center">

**Repositorio del Curso de Alura Latam - Manipulación y Consulta de Datos**

[![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Alura Latam](https://img.shields.io/badge/Plataforma-Alura_Latam-00C86F?style=for-the-badge)](https://www.aluracursos.com/)
[![SQL](https://img.shields.io/badge/Lenguaje-SQL-CC2927?style=for-the-badge)](https://www.w3schools.com/sql/)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-yellow?style=for-the-badge)](LICENSE)

[📥 Instalación](#-instalación-de-mysql-y-workbench) •
[🚀 Primeros Pasos](#-primeros-pasos-con-sql) •
[🗂️ Estructura](#-estructura-del-repositorio) •
[👨‍💻 Autor](#-autor)

</div>

---

## 📚 Descripción del Curso

Este repositorio contiene los archivos, ejercicios y recursos relacionados con el curso **"Introducción a SQL con MySQL: Manipule y consulte datos"** de Alura Latam.

El objetivo del curso es proporcionar los fundamentos prácticos para trabajar con bases de datos relacionales utilizando **MySQL**, uno de los sistemas de gestión de bases de datos relacionales (RDBMS) más populares y ampliamente utilizados en el mundo. Aprenderás a crear, consultar, actualizar y gestionar datos de manera eficaz.

---

## 🛠️ Instalación de MySQL y Workbench

Para comenzar, necesitas instalar el servidor MySQL y MySQL Workbench, una herramienta visual unificada para arquitectos, desarrolladores y DBAs.

### 📥 Guía de Descarga por Sistema Operativo
| Sistema Operativo | Paquete Recomendado | Enlace Directo | Notas |
| :--- | :--- | :--- | :--- |
| **Windows** | MSI Installer (64-bit) | [MySQL Workbench Downloads](https://dev.mysql.com/downloads/workbench/) | Usa el instalador de Windows para una configuración sencilla. |
| **macOS** | macOS Installer (.dmg) | [MySQL Downloads](https://dev.mysql.com/downloads/mysql/) | Sigue la guía de instalación con paquetes nativos. |
| **Linux (Ubuntu/Debian)** | Paquete APT `mysql-workbench-community` | Instalar vía repositorio APT | Asegúrate de instalar el repositorio oficial de MySQL primero. |
| **Linux (RHEL/Fedora)** | Paquete RPM `mysql-workbench-community` | Instalar vía repositorio YUM | Puede requerir acceso al repositorio EPEL. |

> ⚠️ **Nota para Linux:** Las distribuciones de Linux suelen incluir su propia compilación de MySQL Workbench en sus repositorios. Para obtener la versión oficial y más actualizada del equipo de MySQL, se recomienda instalar el repositorio oficial de MySQL (APT o Yum) y luego el paquete `mysql-workbench-community`.

---

## 🚀 Primeros Pasos con SQL

### 1. Conectarse al Servidor MySQL
Después de la instalación, conecta tu cliente (`mysql` o Workbench) al servidor. Usa el usuario `root` y la contraseña que definiste durante la instalación.
```bash
mysql -u root -p
```

### 2. Comandos SQL Fundamentales
SQL (Structured Query Language) es el lenguaje estándar para operar con bases de datos relacionales. Los comandos no son sensibles a mayúsculas.

#### 🗃️ Mostrar y Crear Bases de Datos
```sql
-- Listar todas las bases de datos
SHOW DATABASES;

-- Crear una nueva base de datos
CREATE DATABASE nombre_de_tu_base;
```

#### 📁 Crear una Tabla e Insertar Datos
```sql
-- Seleccionar la base de datos a usar
USE nombre_de_tu_base;

-- Crear una tabla
CREATE TABLE mascotas (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nombre VARCHAR(100) NOT NULL,
    especie VARCHAR(50),
    edad INT
);

-- Insertar un registro
INSERT INTO mascotas (nombre, especie, edad)
VALUES ('Fido', 'Perro', 3);

-- Consultar todos los registros
SELECT * FROM mascotas;
```

#### ✏️ Consultas Básicas y Filtros
```sql
-- Seleccionar columnas específicas
SELECT nombre, edad FROM mascotas;

-- Filtrar resultados con WHERE
SELECT * FROM mascotas WHERE especie = 'Gato';

-- Ordenar resultados
SELECT * FROM mascotas ORDER BY edad DESC;
```

---

## 🗂️ Estructura del Repositorio

```
1790-introduccion-a-sql-con-mysql/
│
├── 📁 ejercicios/          # Scripts SQL con ejercicios prácticos del curso
├── 📁 ejemplos/           # Bases de datos y consultas de ejemplo
├── 📁 recursos/           # Enlaces, cheatsheets y material complementario
├── 📄 README.md           # Este archivo
└── 📄 LICENSE             # Licencia MIT
```

---

## 📖 Recursos de Aprendizaje Recomendados

*   **Documentación Oficial de MySQL**: El mejor recurso para detalles técnicos y referencia.
*   **W3Schools MySQL Tutorial**: Tutorial interactivo con ejemplos y ejercicios para practicar en línea.
*   **MySQL Tutorial**: Un sitio dedicado con guías profundas sobre conceptos avanzados.

---

## 👨‍💻 Autor

<div align="center">

**Darwin Manuel Ovalles Cesar**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Perfil_Profesional-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/darwin-manuel-ovalles-cesar-dev)
[![GitHub](https://img.shields.io/badge/GitHub-Repositorios-black?style=flat&logo=github)](https://github.com/dovalless)

</div>

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

---
**¡Éxitos en tu aprendizaje de SQL! 🎯**
