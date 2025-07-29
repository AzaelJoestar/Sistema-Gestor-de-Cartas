
# MasterDeck - Gestor de Cartas TCG

**Equipo:** #8  
**Integrantes:**  
- Azael Hernández Uvera - Desarrollador y diseñador  
- Isai Raziel Toledo Mariscal - Desarrollador y tester

---

## ¿Qué hace el sistema?

MasterDeck es un sistema de gestión de cartas coleccionables para una biblioteca de juegos TCG.
Permite a los usuarios registrarse, iniciar sesión, visualizar cartas, y administrarlas en un entorno visual amigable.

---

## Tipo de sistema

Aplicación de escritorio (Desktop App) desarrollada en Java (JDK 24) usando Swing para la interfaz gráfica.
Desarrollada en Apache NetBeans IDE 26, con conexión a base de datos MySQL mediante MySQL Workbench 8.0.

---

## Librería externa implementada

- Usamos la librería **[Librería para enviar correo electrónico con PDF o imágenes]
(https://github.com/olmomomo/Libreria_correoElectronico)** del **Equipo 2** para el **registro de usuarios y envío de confirmación por correo**.

---

## Componente visual integrado

- Implementamos el módulo **[JMenuBar Personalizable]
- (https://github.com/Isa-Tomar/JMenuBar-Personalizable)** del **Equipo 8** para una mejor experiencia visual en el menú principal.
- (https://github.com/fergmlx/componente-menu-lateral)** implementacion del componente visual menubar vertical hecho por el **Equipo 3**.
  
---

## Funcionalidades Clave

### 🔐 Integración de CAPTCHA
- El sistema genera un CAPTCHA personalizado al **registrarse un nuevo usuario**, asegurando que el proceso no sea automatizado. 
Se genera una imagen y se valida contra la entrada del usuario.
![vregistro](/Capturas/vregistro.jpg)


### 👥 CRUD de Usuarios
- Registro de nuevos usuarios con correo electrónico y validación visual.
- Inicio de sesión con validación contra base de datos.
- Interfaz de administración para visualizar usuarios.
![tablausuario](/Capturas/tablausuario.jpeg)


### 🃏 CRUD de Cartas
- Alta, edición y eliminación de cartas TCG dentro del sistema.
- Visualización detallada de las cartas con atributos como nombre, tipo, rareza, ataque, defensa e imagen.
![modcarta](/Capturas/modcarta.jpeg)
![tablacarta](/Capturas/tablacarta.jpeg)

### 📬 Envío de Correo Electrónico con Imagen Adjunta
- Al registrarse, el sistema envía una confirmación por correo con imagen adjunta usando **JavaMail** a través de la **librería del equipo 2**.  
![correo](/Capturas/correo.jpeg)

### 🌟 Otras funcionalidades únicas
- Personalización visual con imágenes de fondo en diferentes ventanas.
- Visualización de cartas en una interfaz estilo juego TCG.
- Módulo administrativo con pestañas de gestión de cartas y juegos.
- Visualización de cartas en modo ampliado.
![vercarta](/Capturas/vercarta.jpg)


---

## Dependencias y Configuración

### 📚 Librerías externas usadas
- **JavaMail** (incluido en librería del equipo 2)
- **Librería del Equipo 2** para correos (correo con PDF/imágenes)  
- **JMenuBar del Equipo 8** para menús personalizados
- **JMenuBar del Equipo 3** para menús personalizados verticales

### ⚙️ Pasos para instalar/ejecutar
1. Clonar o descargar el repositorio del proyecto.
2. Descomprimir el achivo login.
3. Al descomprimir veremos otros 2 arvhicos comprimidos, es importante que estos igual se descompriman y las carpetas dentro del archivo comprimido se coloquen dentro de la carpeta login.
4. Abrir el proyecto en NetBeans o IDE compatible con Java.
5. Agregar todas las librerías del proyecto.
6. Ejecutar la clase `Login.java` desde el paquete `login`.
7. Asegurarse de tener base de datos activa y configurada en la librería `LibreriaSQL`.

### 🖥️ Requisitos mínimos
- Java 11 o superior  
- IDE compatible (NetBeans recomendado)  
- Conexión a base de datos MySQL 8.0  
- Acceso a internet para pruebas de envío de correos

---
