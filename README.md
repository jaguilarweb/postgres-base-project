# INTRODUCCIÓN

Este proyecto contiene la configuración base de un proyecto que incluye PostgreSQL.

## Pasos

Crear una carpeta que será el proyecto.

Crear una nueva carpeta llamada ‘src’ 

Crear, dentro de 'src', un archivo index.ts

Inicializar el proyecto con npm ``` npm init -y ```

Agregar typescript con npm ```npm i —save-dev typescript```

Agregar las siguientes librerias:
```npm i --save-dev ts-node```
```npm i —-save-dev @types/node```
```npx tsc —init```

### Configuraciones

En el archivo ***package.json*** crear el script:
> “script:{ “build”: “npx tsc”}

Estar segura de incluir esta configuración en ***tsconfig.json***:
>“target”: “ES5”,

>“module”: “commonjs”,

>“lib”: [“ES6”, “DOM”]

También habilitar:
>“outDir”: “./build”

Asesurarse que las siguientes opciones estén configuradas así:
>“strict”: true,

>“noImplicityAny”: true,

Al final excluir lo siguiente:
>“exclude”: [“node_modules”]


Agregar también las siguientes librerias:
```npm i express```
```npm i @types/express```
```npm i --save-dev tsc-watch```
```npm i body-parser```

## Test Jasmine

Instalar Jasmine

```npm i --save-dev jasmine```

Instalar report Jasmine
``` npm i --save-dev jasmine-spec-reporter```

Instalar difinición de type para Jasmine,
para trabajar con los archivos Jasmine y Typescript 

``` npm i --save-dev @types/jasmine```

``` npm i --save-dev jasmine-ts```

Intalación de librerias de PostgreSQL:

```npm install pg```
```npm install @types/pg```

Librerias migración de BD:
```npm install -g db-migrate```
``` npm install db-migrate db-migrate-pg```

Librería para variables de entorno:

```npm install dotenv```


Usando Docker:

- Instalar docker
- Crear el archivo docker-compose.yml
- Crear las variables de entorno de posgres en .env
- Crear el archivo de conexion de base de datos.
- Ejecutar el comando ```docker-compose up``` para levantar la instancia.
- Inspeccionar si la instancia está corriendo ```docker-compose ps```
- Ejecutar ```docker-compose exec -it <id> bash```
- Para bajar la instancia ```docker-compose down```



Al finalizar compilar con el comando:
```npm run build```