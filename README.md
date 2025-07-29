# Biblioteca Digital

**Número de equipo:** 3

## Integrantes
- Cuevas Estevez Marcos Gabriel - Backend/Frontend
- PerfilGit:
- Galeote Carrera Roman Santiago - Backend/Frontend
- PerfilGit

## ¿Qué hace el sistema?
Sistema que permite la consulta y descarga de libros con api de libros 

## Tipo de sistema
Sistema Web

## Funcionalidades Clave
--------
### 🔐 Proceso de Logueo
El sistema cuenta con autenticación segura con validación de usuario y contraseña.Se usu Sanctum
Antes de iniciar sesión podemos verificar que los campos son validados para que se ingrese un correo y una contraseña (mínimo 6 caracteres)
 <img width="542" height="476" alt="image" src="https://github.com/user-attachments/assets/c35bf3f6-7ceb-4d45-8f9d-d3c5a9f9de6f" />

Iniciamos sesión con el primer usuario que es administrador, al momento de escribir tanto un correo como contraseña validos se habilita el botón de iniciar sesión, también el ojito no permite ocultar la contraseña

<img width="451" height="288" alt="image" src="https://github.com/user-attachments/assets/27db76cb-b6c0-4010-90e8-980bfe458f89" />

### 🔐 Proceso de Registro
Para registrarnos nos dirigimos a la parte inferior
<img width="383" height="59" alt="image" src="https://github.com/user-attachments/assets/69618c2b-b76e-423c-93ba-6433b81bee76" />
Nos mostrará el siguiente formulario que tendrá validaciones iguales al login además de que las contraseñas sean iguales 

--------
### 🧑‍💼 Niveles de Usuario | Rol
- **Administrador**: Acceso completo al sistema (gestión de productos).
<img width="921" height="500" alt="image" src="https://github.com/user-attachments/assets/a24f9386-fa47-4ad7-999b-5702aaa89df0" />
Al registrarnos nos muestra el siguiente mensaje, implementamos un correo de bienvenida para el usuario que se registre
<img width="435" height="462" alt="image" src="https://github.com/user-attachments/assets/df31bacd-0e58-4025-bfca-8d490931d15f" />
El contenido del correo es el siguiente 
<img width="921" height="456" alt="image" src="https://github.com/user-attachments/assets/b39ad528-9fa8-45fc-a665-d71f48392298" />


- **Usuario**: visualización de productos y descarga.
Al iniciar sesión tenemos el catálogo de libros donde tenemos el número total de libros, un navbar que contiene el catálogo, sección de favoritos, buscador y botón de cerrar sesión
<img width="921" height="437" alt="image" src="https://github.com/user-attachments/assets/189210c4-399e-437a-bbf4-8ac793dd2945" />

 <img width="921" height="444" alt="image" src="https://github.com/user-attachments/assets/2ef39467-efe5-410a-a711-f22c80f4d1e9" />
 -Descarga de archivos 
 Podemos descargar los libros usando el botón que lo indica 
<img width="403" height="1071" alt="image" src="https://github.com/user-attachments/assets/c44691df-7ec0-4dce-a9b2-8ba0a689e194" />

### 📦 CRUD de Productos
Gestión completa de libros con campos como nombre, categoría, descripcion, entre otros
- Crear
<img width="921" height="500" alt="image" src="https://github.com/user-attachments/assets/1f942fc7-4bf2-435a-95e3-7ff8d8b3dae3" />
<img width="373" height="626" alt="image" src="https://github.com/user-attachments/assets/d0105f0e-1834-46c8-8706-d4aa7539e59d" />
Al crearlo correctamente nos mostrará el siguiente mensaje y vemos que el libro se añadió correctamente
<img width="231" height="562" alt="image" src="https://github.com/user-attachments/assets/b2468934-58d0-47e4-bc3a-0283f5e918ba" />

- Eliminar
Para eliminar solo daremos click en dicho botón 
<img width="526" height="406" alt="image" src="https://github.com/user-attachments/assets/2a41fb82-916b-4933-9478-18fef0cec9b9" />
<img width="399" height="286" alt="image" src="https://github.com/user-attachments/assets/2361ded1-5fee-46c8-8b4f-2e46f07ddc83" />

- Editar
Para editar un libro de igual manera usamos su respectivo botón, donde de igual manera nos pide validar los campos,
<img width="299" height="458" alt="image" src="https://github.com/user-attachments/assets/cd3441af-7595-40f5-ac7a-903a27746c8e" />
Como vemos los datos se han actualizado correctamente
<img width="230" height="565" alt="image" src="https://github.com/user-attachments/assets/d91e6269-77d2-49a4-9abd-a4b6e4af6433" />

---

### 📧 Envío de Correo Electrónico 
- Al iniciar sesion se envia un pdf de bienvenida
- El PDF se genera usando la librería:swiftmail
- Además de un regalo muy especial, esto es posible mediante la librería Illuminate\Mail que gestiona los correos, SwiftMailer y egulias/email-validator para validar direcciones de correo
- <img width="434" height="229" alt="image" src="https://github.com/user-attachments/assets/cdfef37f-76a9-431d-a1e6-6fb7e65552ba" />


---

### ✨ Otras Funcionalidades Únicas
- **Búsqueda rápida de productos por nombre**
  Tenemos la capacidad de buscar ya sea por nombre, número de libro y coincidencia mas cercana
  <img width="921" height="652" alt="image" src="https://github.com/user-attachments/assets/738161ac-cfc5-49a8-8c32-7fce0f2e45b1" />

- **Paginacion**
  <img width="921" height="467" alt="image" src="https://github.com/user-attachments/assets/e41a7b19-8b43-4aa2-99b8-df0ee5d176c3" />
  <img width="921" height="456" alt="image" src="https://github.com/user-attachments/assets/bd5f1e40-53b9-49e5-8c24-8ee3a0675f0c" />

- **Favoritos**
Para añadir a favoritos solo basta con pulsar el botón de guardar y al seleccionar en el navbar la parte de favoritos nos mandara a nuestro catálogo de favoritos, donde nos mostrará el total de libros favoritos también 
<img width="218" height="581" alt="image" src="https://github.com/user-attachments/assets/377761e8-7059-47a6-b730-189217bcb341" />
<img width="847" height="458" alt="image" src="https://github.com/user-attachments/assets/4302f4a0-dd63-4f70-b751-be3b5a6fd106" />
Para eliminarlo basta con presionar sobre el mismo botón
<img width="921" height="449" alt="image" src="https://github.com/user-attachments/assets/a1c275fa-94be-4493-ae2c-87e5f557c44f" />


---

## Tecnologías Utilizadas
- **Frontend**: HTML, CSS, JavaScript, Bootstrap, Angular  
- **Backend**: PHP, MySQL , laravel
- **Librerías**:swiftmailer
- **Servidor**: XAMPP   
