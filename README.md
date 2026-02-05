# 🎰 Casino Online - Politécnica USAL

Proyecto de desarrollo web para la asignatura **DAW2**. Plataforma de Casino Online completa con funcionalidades sociales y de gamificación, construida sobre el framework Yii2.

## 📋 Descripción del Proyecto
Este sistema simula un entorno de casino real donde los usuarios pueden registrarse, gestionar su monedero virtual, jugar a diversos juegos de azar, participar en torneos y socializar a través de mesas privadas con chat en tiempo real.

El proyecto integra tres módulos principales:
- **Juegos (Casino)**: Lógica de servidor y cliente.
- **Social**: Interacción entre usuarios.
- **Gamificación**: Retención y competición.

## 🚀 Funcionalidades Principales

### 1. Juegos de Azar (Módulo G3/G4)
- **Tragamonedas (Slots)**: Juego visual con cálculo de premios en servidor.
- **Ruleta**: Apuestas a número, color y paridad.
- **Blackjack**: Juego de cartas contra el Dealer con lógica de plantarse/pedir.
- **Seguridad**: Todas las validaciones de saldo y premios ocurren en el Backend para evitar trampas.

### 2. Social (Módulo G6)
- **Mesas Privadas**: Los usuarios pueden crear mesas con contraseña para jugar en grupo.
- **Sala de Chat**: Chat en tiempo real dentro de las mesas privadas.
- **Moderación**: Filtro de palabras ofensivas y control de acceso.

### 3. Gamificación (Módulo W6/G5)
- **Torneos**: Competiciones activas donde los juegos suman puntos al ranking.
- **Logros**: Sistema de medallas por hitos (ej. "Primera Victoria", "Gran Apostador").
- **Economía**: Sistema robusto de Monedero y Transacciones (Historial de depósitos y apuestas).

## 📂 Estructura del Proyecto
El proyecto está organizado en 4 directorios principales:

- **`codigo/`**: Contiene todo el código fuente de la aplicación (Controladores, Modelos, Vistas).
  - `controllers/`: Lógica de negocio (`JuegoController`, `MesaPrivadaController`, etc.).
  - `models/`: Representación de datos (`Usuario`, `Transaccion`, `Logro`, etc.).
  - `views/`: Interfaz de usuario (HTML/PHP).
  - `config/`: Archivos de configuración de BD y parámetros.
- **`sql/`**: Scripts de Base de Datos.
  - `casido_db.sql`: Script principal para importar la estructura y datos iniciales.
- **`librerias/`**: Dependencias externas del proyecto (Vendor).
- **`proyecto/`**: Documentación adicional y recursos del proyecto.

## 🛠️ Guía de Instalación

### Requisitos previos
- Servidor Web (Apache/Nginx).
- PHP 7.4 o superior.
- MySQL / MariaDB.

### Pasos
1.  **Desplegar ficheros**: Copia los archivos del proyecto a tu servidor web (o carpeta `htdocs`).
2.  **Base de Datos**:
    - Crea una base de datos vacía (ej. `casino_db`).
    - Importa el archivo `sql/casido_db.sql` en tu gestor de BD.
3.  **Configuración**:
    - Abre el archivo `codigo/config/db.php`.
    - Ajusta las credenciales (`dsn`, `username`, `password`) para conectar a tu BD local.
4.  **Ejecutar**:
    - Accede a la carpeta `codigo/web/` desde tu navegador.
    - Ejemplo: `http://localhost/Casino_Online/codigo/web/`

## 👤 Usuarios de Prueba
(Consultar base de datos para credenciales específicas, por defecto suele haber un usuario `admin` / `admin` o similar en entornos de desarrollo).

---
*Proyecto realizado para la Universidad de Salamanca - Escuela Politécnica Superior de Zamora.*
