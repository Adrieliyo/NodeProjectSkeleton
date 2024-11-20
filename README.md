# NodeProjectSkeleton

Este es un proyecto base para Node.js que incluye una configuración inicial con las dependencias más comunes para el desarrollo de APIs REST.

## Requisitos Previos

- Node.js instalado en tu sistema
- npm (Node Package Manager)

## Instalación Rápida

Para instalar todas las dependencias de una sola vez, ejecuta:

```bash
npm i
```

## Instalación Paso a Paso

Si prefieres realizar la instalación paso a paso:

1. Inicializar el proyecto npm:
```bash
npm init -y
```

2. Instalar las dependencias necesarias:
```bash
npm install express morgan cors dotenv nodemon bcrypt jsonwebtoken
```

## Dependencias Incluidas

- **express**: Framework web rápido y minimalista para Node.js
- **morgan**: Middleware de logging para HTTP
- **cors**: Middleware para habilitar CORS (Cross-Origin Resource Sharing)
- **dotenv**: Carga variables de entorno desde un archivo .env
- **nodemon**: Utilidad que monitorea cambios en los archivos y reinicia automáticamente el servidor
- **bcrypt**: Librería para el hash de contraseñas
- **jsonwebtoken**: Implementación de JSON Web Tokens

## Estructura del Proyecto

El proyecto sigue una estructura básica recomendada para aplicaciones Node.js:

```
NodeProjectSkeleton/
├── node_modules/
├── src/
│   ├── app/
│   ├── config/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── services/
│   └── utils/
├── test/
├── .env
├── .gitignore
└── package.json
```

## Scripts Disponibles

En el `package.json` se incluyen los siguientes scripts:

```json
{
  "scripts": {
    "start": "node src/app.js",
    "dev": "nodemon src/app.js"
  }
}
```

## Uso

1. Clona este repositorio
2. Instala las dependencias
3. Crea un archivo `.env` basado en `.env.example`
4. Ejecuta el servidor:
   - Para desarrollo: `npm run dev`
   - Para producción: `npm start`