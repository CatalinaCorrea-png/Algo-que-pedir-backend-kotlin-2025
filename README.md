# 🛠️ Algo-que-pedir-backend-kotlin-2025
*Trabajo práctico de la materia Algoritmos III - Tecnicatura en Programación Informática - UNSAM 2C 2025.*

**Backend API en Kotlin con Spring Boot** – una aplicación RESTful construida para el proyecto académico ***Algo que pedir***. Esta API sirve como backend para funcionalidades de manejo de datos y lógica de negocio, usando Spring Boot + Kotlin para un desarrollo moderno, seguro y escalable.

---
### 🚀 Features

✔ Construido con Kotlin + Spring Boot </br>
✔ API REST para manejar recursos backend </br>
✔ Estructura limpia con capas (Controller, Service, Repository) </br>
✗ Integración con base de datos (Repositorios en memoria) </br>
✔ Pruebas y configuración listos para usar </br>
✔ CI/CD con GitHub Actions configurado </br>

---
### 🧱 Arquitectura

Este proyecto utiliza patrones comunes en aplicaciones backend con Spring Boot:
```nginx
Controller → Service → Repository → Data en memoria runtime
```

- **Controller**: define los endpoints HTTP
- **Service**: comunicacion con repositorio y validacion de datos
- **Repository**: Modelo de base de datos. Guarda datos en memoria (Sin motor de base de datos)
- **Model**: contiene lógica de negocio y patrones de diseño. Representan los datos almacenados.

---
### 📦 Tech Stack
| **Tecnología**  	|  Versión / Rol 	| 
|---	|---	|
|  **Kotlin** 	|  Lenguaje principal 	|  
|  **Spring Boot** 	|  Framework principal 	|  
|   **Spring Web**	|   Construcción de API REST	|  
|   **Gradle**	|   Build tools	|  
|   **Spring Web**	|   Testing	|  

---
### 🏁 Comenzando
**Pre-requisitos**

Asegúrate de tener instalado:
- JDK 17 o superior
- Gradle
- (Opcional) Postman o REST client para probar endpoints

---
### 🧾 Instalación

1. **Clonar el repositorio**
```bash
git clone https://github.com/CatalinaCorrea-png/Algo-que-pedir-backend-kotlin-2025.git
cd Algo-que-pedir-backend-kotlin-2025
```

2. **Construir el proyecto**

```bash
./gradlew clean build
```
3. **Ejecutar el backend**
```bash
./gradlew bootRun
```
El servidor levantará en: http://localhost:9000

---
### 🌐 Endpoints API (Ejemplos)

| Método  |	Ruta  |	Descripción | Tipo de Usuario(*) |
|--- |--- |--- |--- |
| GET |	/pedidos/ |	Lista todos los pedidos | Cliente |
| GET |	/pedido/{id} |	Busca pedido por ID | Cliente |
| GET |	/pedidos-usuario/ |	Busca pedidos del usuario por su email (RequestParam) | Cliente |
| POST  |	/create-order/  |	Crea un nuevo pedido  | Cliente |
| PUT |	/preparar_pedido/{id}} |	Actualiza el estado del pedido a preparado  | Local |
| DELETE  |	/eliminar-ingrediente/{id} |	Elimina ingrediente | Local |

- (*) Esta aplicacion funciona como backend para dos interfaces/aplicaciones web: Una destinada al Cliente y otra destinada a el Local/Restaurante
---
### 🧪 Testing

Este proyecto incluye tests automatizados.

Ejecutar tests:
```bash
./gradlew test
```

---
### 📦 Base de Datos

Este proyecto no cuenta con integracion a base de datos. La información es almacenada en tiempo de compilación (memoria) dentro de los repositorios.

---
### 📘 Información Extra

✔ Usa DTOs para separar entidades de API

✔ Maneja y mapea excepciones con controladores globales

✔ Logica de negocio que sigue Patrones de Diseño como Strategy, Composite, Template Method, Observers.

✔ Tests unitarios + de integración 

---
### 💻 **Desarrolladores**
- Catalina Correa
- Nicolas Cernadas
- Dana Cossettini Reyes 
- Maximiliano Andres Bianchimano 
- Fernanda Perez

---
### 📬 **Contacto**

👩‍💻 **Catalina Correa** – Estudiante de informática / Desarrolladora - 📧 catalinayazmincorrea@gmail.com

