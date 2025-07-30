
# Biblioteca Digital

**Número de equipo:** 3

## Integrantes
- Cuevas Estevez Marcos Gabriel - Backend/Frontend  
  - PerfilGit:  https://github.com/Marquitos5555
- Galeote Carrera Roman Santiago - Backend/Frontend  
  - PerfilGit:  https://github.com/RSGALEOTE

## ¿Qué hace el sistema?
Sistema que permite la consulta y descarga de libros con API de libros.

## Tipo de sistema
Sistema Web

## Funcionalidades Clave

---

### 🔐 Proceso de Logueo
El sistema cuenta con autenticación segura con validación de usuario y contraseña. Se usa Sanctum.  
Antes de iniciar sesión podemos verificar que los campos son validados para que se ingrese un correo y una contraseña (mínimo 6 caracteres)  
![Login Validación](https://github.com/user-attachments/assets/c35bf3f6-7ceb-4d45-8f9d-d3c5a9f9de6f)

Iniciamos sesión con el primer usuario que es administrador, al momento de escribir tanto un correo como contraseña válidos se habilita el botón de iniciar sesión, también el ojito permite ocultar la contraseña.  
![Login Admin](https://github.com/user-attachments/assets/27db76cb-b6c0-4010-90e8-980bfe458f89)

### 📝 Proceso de Registro
Para registrarnos nos dirigimos a la parte inferior.  
![Registro Enlace](https://github.com/user-attachments/assets/69618c2b-b76e-423c-93ba-6433b81bee76)  
Nos mostrará el siguiente formulario que tendrá validaciones iguales al login, además de que las contraseñas sean iguales.  

---

### 🧑‍💼 Niveles de Usuario | Rol

- **Administrador**: Acceso completo al sistema (gestión de productos).  
  ![Vista Admin](https://github.com/user-attachments/assets/a24f9386-fa47-4ad7-999b-5702aaa89df0)  
  Al registrarnos nos muestra el siguiente mensaje, e implementamos un correo de bienvenida.  
  ![Mensaje Bienvenida](https://github.com/user-attachments/assets/df31bacd-0e58-4025-bfca-8d490931d15f)  
  El contenido del correo es el siguiente:  
  ![Correo Bienvenida](https://github.com/user-attachments/assets/b39ad528-9fa8-45fc-a665-d71f48392298)

- **Usuario**: Visualización de productos y descarga.  
  ![Vista Usuario](https://github.com/user-attachments/assets/189210c4-399e-437a-bbf4-8ac793dd2945)  
  ![Navbar Usuario](https://github.com/user-attachments/assets/2ef39467-efe5-410a-a711-f22c80f4d1e9)  
  Descarga de archivos:  
  ![Descarga PDF](https://github.com/user-attachments/assets/c44691df-7ec0-4dce-a9b2-8ba0a689e194)

### 📦 CRUD de Productos

Gestión completa de libros con campos como nombre, categoría, descripción, entre otros.

- **Crear**  
  ![Formulario Crear](https://github.com/user-attachments/assets/1f942fc7-4bf2-435a-95e3-7ff8d8b3dae3)  
  ![Validaciones Crear](https://github.com/user-attachments/assets/d0105f0e-1834-46c8-8706-d4aa7539e59d)  
  Al crearlo correctamente, se muestra un mensaje de éxito.  
  ![Mensaje Crear](https://github.com/user-attachments/assets/b2468934-58d0-47e4-bc3a-0283f5e918ba)

- **Eliminar**  
  ![Eliminar Libro](https://github.com/user-attachments/assets/2a41fb82-916b-4933-9478-18fef0cec9b9)  
  ![Confirmar Eliminar](https://github.com/user-attachments/assets/2361ded1-5fee-46c8-8b4f-2e46f07ddc83)

- **Editar**  
  ![Editar Formulario](https://github.com/user-attachments/assets/cd3441af-7595-40f5-ac7a-903a27746c8e)  
  ![Mensaje Editar](https://github.com/user-attachments/assets/d91e6269-77d2-49a4-9abd-a4b6e4af6433)

---

### 📧 Envío de Correo Electrónico

- Al iniciar sesión se envía un PDF de bienvenida.  
- El PDF se genera usando la librería **SwiftMailer**.  
- También se utiliza `Illuminate\Mail` y `egulias/email-validator` para validar direcciones.  
  ![Correo PDF](https://github.com/user-attachments/assets/cdfef37f-76a9-431d-a1e6-6fb7e65552ba)

---

### ✨ Otras Funcionalidades Únicas

- **Búsqueda rápida de productos por nombre, ID y coincidencias**  
  ![Buscador](https://github.com/user-attachments/assets/738161ac-cfc5-49a8-8c32-7fce0f2e45b1)

- **Paginación**  
  ![Paginación 1](https://github.com/user-attachments/assets/e41a7b19-8b43-4aa2-99b8-df0ee5d176c3)  
  ![Paginación 2](https://github.com/user-attachments/assets/bd5f1e40-53b9-49e5-8c24-8ee3a0675f0c)

- **Favoritos**  
  Para añadir a favoritos solo pulsa el botón de guardar. En el navbar se puede acceder a favoritos y ver el total.  
  ![Agregar a Favoritos](https://github.com/user-attachments/assets/377761e8-7059-47a6-b730-189217bcb341)  
  ![Catálogo Favoritos](https://github.com/user-attachments/assets/4302f4a0-dd63-4f70-b751-be3b5a6fd106)  
  Para eliminar, presiona nuevamente el botón.  
  ![Eliminar Favorito](https://github.com/user-attachments/assets/a1c275fa-94be-4493-ae2c-87e5f557c44f)

  -**CRUD para usuarios**
  Solo lo podemos realizar si ingresamos como administrador, tendremos la siguiente opción al lados de favoritos
  <img width="457" height="80" alt="image" src="https://github.com/user-attachments/assets/52afdede-76fc-4151-99f3-b0cad218feab" />
  Una vez presionamos nos dirigirá a la siguiente tabla que contendra todos los usuarios
  <img width="1546" height="416" alt="image" src="https://github.com/user-attachments/assets/e4716f28-4279-4588-af2c-c5eb5d4cc252" />
  Al actualizar un usuario podemos modificar el nombre, correo y rol
  <img width="568" height="444" alt="image" src="https://github.com/user-attachments/assets/eaaca021-2d05-41d1-a01a-059604c4f62b" />
  <img width="564" height="366" alt="image" src="https://github.com/user-attachments/assets/fe3f0bdd-0b1b-4fe6-a592-0b24621bc12e" />
  <img width="1484" height="390" alt="image" src="https://github.com/user-attachments/assets/a8336d53-0509-4d75-96b6-012c4af7abf4" />
  Ahora eliminaremos el último usuario
  <img width="545" height="343" alt="image" src="https://github.com/user-attachments/assets/fb1474f7-5309-4e32-a4b2-7730a4858a81" />
  <img width="507" height="356" alt="image" src="https://github.com/user-attachments/assets/972f9bae-29c7-40e0-8712-1300e0305caf" />
  Como vemos se ha eliminado correctamente
  <img width="1461" height="328" alt="image" src="https://github.com/user-attachments/assets/2cf322d5-de3a-4695-b27d-85c3733ba28c" />
  Al añadir nos pedirá completar todos los campos
  <img width="507" height="585" alt="image" src="https://github.com/user-attachments/assets/ce7460a4-d227-4dbd-a356-6603003d83e4" />
  Al añadirlos solo le daremos click en crear
  <img width="571" height="527" alt="Captura de pantalla 2025-07-29 174130" src="https://github.com/user-attachments/assets/1abb99b6-028a-4333-91cc-6460c277896b" />
  <img width="577" height="359" alt="image" src="https://github.com/user-attachments/assets/2e2e553d-8a42-4c5e-86c6-d4e86714a1c7" />
  Vemos que se añadió correctamente
  <img width="1510" height="406" alt="image" src="https://github.com/user-attachments/assets/d124bef9-ebed-4419-b35c-622c60b4f8d4" />
  Cabe resaltar que aal crear un usuario desde aquí el correo también es enviado al usuario registrado
  <img width="1416" height="658" alt="Captura de pantalla 2025-07-29 174407" src="https://github.com/user-attachments/assets/46b3c910-f189-4932-acb0-a6e6f0ad5425" />
  Ahora iniciamos sesión con este nuevo usuario para comprobar que sus credenciales son validas
  <img width="541" height="430" alt="image" src="https://github.com/user-attachments/assets/6596ce93-e211-4a99-9299-59f6eff64687" />
  <img width="1784" height="854" alt="image" src="https://github.com/user-attachments/assets/9cbbc6bb-a82c-4e44-909a-730a1edae7e5" />
  Tambíen tenemos la función de eliminar cuenta
  <img width="338" height="284" alt="image" src="https://github.com/user-attachments/assets/73363bfa-382f-4b1d-98f2-01057a9a84c4" />
  <img width="556" height="356" alt="image" src="https://github.com/user-attachments/assets/d29f9592-b1b0-419e-bb10-690f47fcd00b" />
  Como vemos la ha eliminado correctamente además nos regresa al login en automático, también lo verificamo en la base de datos 
  <img width="1818" height="873" alt="image" src="https://github.com/user-attachments/assets/86676c00-8777-494e-9507-82c65b8ca0d1" />
  <img width="1119" height="163" alt="image" src="https://github.com/user-attachments/assets/eb804dae-9bd2-4a3f-8f79-5a6fde0c9060" />
---

## Tecnologías Utilizadas

- **Frontend**: HTML, CSS, JavaScript, Bootstrap, Angular  
- **Backend**: PHP, MySQL, Laravel  
- **Librerías**: SwiftMailer, Illuminate\Mail  
- **Servidor**: XAMPP
