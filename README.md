# 📚 Challenge Literalura - Oracle Next Education & Alura Latam

Este proyecto corresponde al **Challenge Literalura**, parte de la formación en **Spring Boot** del programa **Oracle Next Education (ONE)** en conjunto con **Alura Latam**.

El desafío consiste en implementar una aplicación que consuma la API de **Gutendex**, permitiendo gestionar un catálogo de libros y autores, almacenándolos en una base de datos relacional y ofreciendo funcionalidades de consulta.

---

## 🚀 Tecnologías utilizadas

- **Java 17**
- **Spring Boot 3**
- **Spring Data JPA**
- **Hibernate**
- **PostgreSQL** (o MySQL)
- **Gutendex API** (https://gutendex.com/books/)
- **Maven**
- **IntelliJ IDEA / Eclipse**

---

## 📌 Funcionalidades principales

✔️ Buscar libros por título en la API Gutendex  
✔️ Guardar libros y autores en la base de datos  
✔️ Listar libros registrados  
✔️ Listar autores registrados  
✔️ Consultar autores vivos en un año específico  
✔️ Consultar libros por idioma  
✔️ Evitar duplicados en el registro de libros/autores  

---

## 📂 Estructura del proyecto

```
src/
 ├── main/
 │   ├── java/com/literalura/
 │   │   ├── controller/   # Controladores REST
 │   │   ├── model/        # Entidades JPA
 │   │   ├── repository/   # Repositorios
 │   │   ├── service/      # Lógica de negocio
 │   │   └── LiteraluraApplication.java
 │   └── resources/
 │       ├── application.properties
 │       └── data.sql / schema.sql
 └── test/
```

---

## ⚙️ Configuración

En `application.properties` debes configurar la conexión a tu base de datos:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/literalura
spring.datasource.username=postgres
spring.datasource.password=tu_contraseña

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

---

## ▶️ Ejecución

1. Clonar el repositorio  
2. Configurar la base de datos en `application.properties`  
3. Ejecutar la aplicación con:  

```bash
mvn spring-boot:run
```

4. Usar los endpoints expuestos en **Postman** o cualquier cliente REST.

---

## 🧪 Ejemplos de consultas

- Buscar libros: `/api/libros?titulo=Don Quijote`  
- Listar autores vivos en 1900: `/api/autores?vivosEn=1900`  
- Listar libros por idioma: `/api/libros?idioma=es`  

---

## 🎯 Objetivo del Challenge

Este reto busca aplicar conocimientos de:

- **Consumo de APIs REST**
- **Persistencia de datos con Spring Data JPA**
- **Modelado de entidades**
- **Buenas prácticas en Spring Boot**

---

## 👩‍💻 Autor

**Jenny Joseline Mamani Choque**  
📧 [yenny501ss@gmail.com](mailto:yenny501ss@gmail.com)  
💼 [LinkedIn](https://www.linkedin.com/in/jenny-joseline-mamani-choque-07963593)

---

✨ Este proyecto forma parte del programa **Oracle Next Education (ONE) + Alura Latam**.  
