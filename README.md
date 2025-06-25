# App FullStack - Gestión de Productos (UTN)

Este proyecto es una aplicación fullstack que permite realizar un CRUD (Crear, Leer, Actualizar, Eliminar) de productos utilizando MongoDB, Express, React y Node.js.

## Nueva funcionalidad agregada

Se ha implementado una **búsqueda por nombre de producto**, que permite al usuario buscar coincidencias parciales desde el frontend. Esta búsqueda se realiza de forma insensible a mayúsculas/minúsculas y es procesada por el backend a través de una ruta específica.

---

## Tecnologías utilizadas

### Backend

* Node.js
* Express
* MongoDB
* Mongoose
* dotenv
* TypeScript

### Frontend

* React
* Vite
* Axios
* React Router DOM
* CSS

---

## Instrucciones para ejecutar el proyecto

### Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/app-utn-final.git
cd app-utn-final
```

### Backend

```bash
cd backend
npm install
cp .env.example .env
npm run dev
```

### Frontend

```bash
cd frontend
npm install
cp .env.example .env
npm run dev
```

---

## Ejemplo de uso de la nueva funcionalidad

1. Ir a la pantalla principal donde se listan los productos.
2. Utilizar el input superior: "Buscar productos por nombre...".
3. Al tipear una palabra, los productos mostrados se filtrarán en tiempo real desde el backend.

---

## Variables de entorno necesarias

### backend/.env

```
PORT=1234
URI_DB=mongodb://localhost:27017/api-auth
JWT_SECRET=aguanteboca
```

### frontend/.env

```
VITE_BACKEND_URL=http://localhost:1234
```

---

## Notas adicionales

* Asegurarse de que MongoDB esté corriendo localmente o tener acceso a una URI válida.
* Las rutas están protegidas por autenticación JWT.
* Se incluye validación de sesión al momento de realizar búsquedas o acciones CRUD.

---
Autor:
Desarrollado por Andrés González – Curso Backend UTN.BA