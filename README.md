# 🌍 ProyectoFinal - Sistema de Consulta de Sismos

Este proyecto es una aplicación web desarrollada con Spring Boot que permite a los usuarios registrarse, iniciar sesión, editar su perfil, consultar información y simular sismos en un mapa interactivo. Está orientado a brindar una interfaz sencilla y útil para visualizar eventos sísmicos ocurridos en México.

## 🚀 Tecnologías utilizadas

- Java 17  
- Spring Boot  
- Spring Security  
- Thymeleaf  
- MySQL  
- Maven  
- HTML + CSS (con soporte para tema claro/oscuro)  
- Leaflet.js (para el mapa interactivo)

## 🧑‍💻 Funcionalidades principales

- Registro y login de usuarios con roles (`USER`, `ADMIN`)  
- Edición de perfil de usuario (nombre, correo, contraseña)  
- Selector de tema claro/oscuro con persistencia en base de datos  
- Visualización de sismos en un mapa con marcadores personalizados  
- Simulación de sismos en un mapa interactivo
- CRUD de usuarios para administradores
- CRUD de sismos para administradores

---

## ⚙️ Instalación

### 1. Clona el repositorio

```bash
git clone https://github.com/tu-usuario/ProyectoFinal.git
cd ProyectoFinal
```

### 2. Configura la base de datos

Asegúrate de tener un servidor **MySQL** corriendo 

Importa el archivo `proyectofinal.sql` 

```bash
mysql -u tu_usuario -p proyectofinal_db < proyectofinal.sql
```

### 3. Configura el archivo `application.properties`

Edita el archivo `src/main/resources/application.properties` con tus credenciales:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/proyectofinal_db
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### 4. Compila el proyecto

```bash
./mvnw clean install
```

> Si estás en Windows, usa `mvnw.cmd` en lugar de `./mvnw`.

---

## ▶️ Ejecución

Ejecuta la aplicación con el siguiente comando:

```bash
./mvnw spring-boot:run
```

La aplicación estará disponible en:

```
http://localhost:8080/login
```

---

## 👤 Credenciales de prueba

**Administrador**  
- Correo: sebas@gmail.com  
- Contraseña: sebas


---

