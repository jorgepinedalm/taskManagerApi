# 📝 API de Gestión de Tareas (Backend - .NET 8)

Este es el backend desarrollado en **.NET Core 8** para gestionar tareas mediante una API RESTful. La API permite **crear, listar, actualizar y eliminar tareas** (CRUD) y utiliza **Entity Framework Core** con una base de datos en memoria.

---

## 🚀 Características

- ✅ API RESTful para gestionar tareas.  
- ✅ CRUD de tareas (crear, leer, actualizar, eliminar).  
- ✅ Uso de **Entity Framework Core** con una base de datos en memoria.  
- ✅ Configuración de **CORS** para permitir el acceso desde el frontend.  
- ✅ Endpoints bien estructurados y documentados.  
- ✅ Desarrollado con buenas prácticas en .NET 8.

## 🛠️ Tecnologías Usadas

✅ **.NET 8**  
✅ **ASP.NET Core Web API**  
✅ **Entity Framework Core** 


## 📦 Instalación y Configuración

### 🔹 1. Clonar el Repositorio

```sh
git clone https://github.com/jorgepinedalm/taskManagerApi.git
cd taskManagerApi
```

### 🔹 2. Requisitos Previos

Asegúrese de tener instalado:
- **.NET 8 SDK** → [Descargar aquí](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
- **Visual Studio 2022** con la carga de trabajo **ASP.NET y desarrollo web**

### 🔹 3. Restaurar Dependencias

Ejecute el siguiente comando para restaurar las dependencias del proyecto:

```sh
dotnet restore
```

### 🔹 4. Ejecutar la Aplicación

Ejecute el siguiente comando para iniciar el servidor:

```sh
dotnet run
```

Por defecto, la API estará disponible en:
```
https://localhost:44320/api/tasks
```

Si la dirección es diferente, actualice la **URL base** en el frontend (`src/environments/environment.ts`).

---

## 📑 Endpoints Disponibles

| Método   | Endpoint          | Descripción              |
| -------- | ----------------- | ------------------------ |
| `GET`    | `/api/tasks`      | Obtener todas las tareas |
| `POST`   | `/api/tasks`      | Crear una nueva tarea    |
| `PUT`    | `/api/tasks/{id}` | Actualizar una tarea     |
| `DELETE` | `/api/tasks/{id}` | Eliminar una tarea       |

---

## 🔌 Conexión con el Frontend

Para conectar el frontend con este backend, asegúrese de configurar correctamente la **URL base** en el archivo:

📂 **src/environments/environment.ts** (en el proyecto Angular)
```ts
export const environment = {
  production: false,
  apiUrl: 'https://localhost:44320/api/tasks'
};
```

Si el backend se ejecuta en otro puerto o dominio, modifica este valor.

---

## 🌍 Despliegue (Opcional)

El despliegue para el backend se realiza a través del asistente de Visual Studio desde el cual se tiene acceso a la suscripción de la cuenta con la que se creó el recurso donde se desplegó la aplicación. Puede tener acceso a la aplicación desplegada desde: 
[https://taskmanagerapi20250313114734-hrehhsgzfzezhwdv.eastus-01.azurewebsites.net/api/tasks](https://taskmanagerapi20250313114734-hrehhsgzfzezhwdv.eastus-01.azurewebsites.net/api/tasks)

## 🎯 Mejoras Futuras (Extras)

- ⭐ Validaciones en los modelos para evitar datos incorrectos.  
- ⭐ Implementación de **Autenticación y Autorización**.  
- ⭐ Uso de una base de datos **SQL Server o SQLite** en lugar de en memoria.  
- ⭐ Pruebas unitarias con **xUnit** o **MSTest**.  

## 💡 Contacto

Si tienes dudas o sugerencias, contáctame en **[LinkedIn](https://www.linkedin.com/in/jorgepinedam/)**.

🚀 *¡Gracias por revisar este proyecto!* 🚀
