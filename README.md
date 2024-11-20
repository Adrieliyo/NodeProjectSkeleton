# NodeProjectSkeleton

Este es un proyecto base para Node.js que incluye una configuración inicial con las dependencias más comunes para el desarrollo de APIs REST.

## Requisitos Previos

- Node.js instalado en tu sistema
- npm (Node Package Manager)
- Git instalado en tu sistema

## Primeros Pasos

1. Clonar el repositorio:
```bash
git clone https://github.com/Adrieliyo/NodeProjectSkeleton.git
```

2. Entrar al directorio del proyecto:
```bash
cd repositorio-original-clonado
```

3. Debes desvincular el repositorio clonado del remoto original para evitar confusiones. Puedes verificar el origen actual con:
```bash
git remote -v
```

4. Eliminar la referencia al repositorio remoto original:
```bash
git remote remove origin
```

5. Ve a GitHub y crea un nuevo repositorio.

6. No inicialices el repositorio con un archivo README, .gitignore o licencia, ya que esto podría generar conflictos.

7. Agregar tu propio repositorio remoto:
```bash
git remote add origin https://github.com/tu-usuario/tu-repositorio.git
```

8. Subir los cambios a tu repositorio
Primero, verifica que el nuevo remoto está configurado correctamente:
```bash
git remote -v
```
Luego, sube los archivos al nuevo repositorio:
```bash
git branch -M main # Renombra la rama principal a 'main' si es necesario
git push -u origin main
```

9. Confirmar que el repositorio se subió correctamente
Ve a la página de tu nuevo repositorio en GitHub y verifica que el contenido del repositorio se haya cargado.

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


