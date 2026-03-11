# PHP Authentication System (Login & Register)

Este proyecto es un sistema de gestión de acceso de usuarios enfocado en la seguridad y la modularidad. Implementa un flujo completo de autenticación, desde el registro de usuarios con contraseñas encriptadas hasta el manejo de sesiones persistentes.

---

## CARACTERÍSTICAS TÉCNICAS
* **Lógica del Servidor:** PHP 8.2 con arquitectura modular (uso de carpetas `includes`).
* **Seguridad:** Implementación de sentencias preparadas (Prepared Statements) para prevenir inyecciones SQL.
* **Cifrado:** Almacenamiento de credenciales mediante el algoritmo de hashing BCRYPT (`password_hash`).
* **Persistencia:** Gestión de sesiones de usuario con `session_start` y `session_destroy`.
* **Frontend:** Interfaz responsiva basada en Bootstrap 5.

## REQUISITOS DE EJECUCIÓN
Para correr este proyecto localmente, se requiere un entorno de servidor WAMP/XAMPP:

1. Clonar este repositorio en la carpeta `htdocs`.
2. Iniciar los módulos **Apache** y **MySQL** desde el Panel de Control de XAMPP.
3. Crear una base de datos llamada `auth-sys` en phpMyAdmin.
4. Importar el archivo `auth-sys.sql` incluido en la raíz de este proyecto.

## ESTRUCTURA DE ARCHIVOS
* `config.php`: Configuración centralizada de la conexión PDO.
* `register.php`: Lógica de validación e inserción de nuevos usuarios.
* `login.php`: Validación de credenciales y apertura de sesiones.
* `includes/`: Componentes reutilizables de la interfaz (Header y Footer).

---
**Desarrollado por Diego Mamani** | Sistemas y Programación - UMECIT
