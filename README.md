# Biblioteca Digital

**Número de equipo:** 3

## Integrantes
- Cuevas Estevez Marcos Gabriel - Backend/Frontend
- Galeote Carrera Roman Santiago - Backend/Frontend

## ¿Qué hace el sistema?
Sistema que permite la consulta y descarga de libros 

## Tipo de sistema
Sistema Web

## Funcionalidades Clave

### 🔐 Proceso de Logueo
El sistema cuenta con autenticación segura con validación de usuario y contraseña.Se usu Sanctum


### 🧑‍💼 Niveles de Usuario | Rol
- **Administrador**: Acceso completo al sistema (gestión de productos).

- **Usuario**: visualización de productos y descarga.


### 📦 CRUD de Productos
Gestión completa de productos con campos como nombre, categoría, descripcion, entre otros




### 🛒 Proceso Principal: Venta de Productos
- El cajero selecciona productos desde una interfaz amigable.
- Se calculan los totales automáticamente.
- Se genera un ticket digital al finalizar la venta.

![Venta de Productos](imagenes/venta.png)

---

### 📧 Envío de Correo Electrónico con PDF adjunto
- Al iniciar sesion se envia un pdf de bienvenida
- El PDF se genera usando la librería:

---

### ✨ Otras Funcionalidades Únicas
- **Búsqueda rápida de productos por nombre**
- 
- **Paginacion**

---

## Tecnologías Utilizadas
- **Frontend**: HTML, CSS, JavaScript, Bootstrap  
- **Backend**: PHP, MySQL  
- **Librerías**: DOMPDF, PHPMailer  
- **Servidor**: XAMPP / Apache  
