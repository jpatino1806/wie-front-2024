# Frontend | Plataforma iot

<div style="text-align: center">
<!--     <img src="https://academy.dignal.com/wp-content/uploads/2023/01/dignal_academy_logo_site.png" width="400" alt="Dignal Academy"/> -->
    <img src="https://academy.dignal.com/wp-content/uploads/2023/01/dignal_academy_logo_site.png" width="400" alt="Dignal Academy"/>    
</div>

## Contenido

Este repositorio contiene el frontend de nuestra plataforma iot, diseñada con vue3 y vuetify.

## INICIO E INSTALACION DEL PROYECTO

- Si eres usuario windows primero debes instalar WSL en la PC, la cual va a instalar una distribucion de Ubuntu dentro de windows10 es como si tuvieramos otra PC con UBUNTU dentro de windows10.
- Despues instalar docker desktop en tu PC.
- En la terminal entrar a ubuntu luego /home/jpatino y ahi crear una carpeta llamada **wie-plataforma-iot** y alli debes ***clonar***  las dos carpetas del proyecto 
  ```
     git clone https://github.com/Dignal-Electronics/iot-backend-2024.git
  ```
  ```
	 git clone https://github.com/Dignal-Electronics/iot-front-2024.git
  ```
- Cambiamos el nombre de las carpetas:
	- iot-backend-2024 por  **wie-backend-2024**
	- iot-front-2024   por  **wie-frontend-2024**

- En la terminal de visual code iniciamos el repositorio con el comando
  ```
  git init
  git add .
  git commit -m "primer commit"
  ```
- Luego deber ir al navegador y en github deberas crear un repositorio nuevo para enviar tu proyecto al repositorio de github. 
  ```
  git remote add origin https://github.com/jpatino1806/wie-iot-2024.git
  git push origin master
  ```
  * despues solo debes actualizar hasta el fin del tu proyecto.

## LEVANTAR EL PROYECTO CON DOCKER

- El proyecto debe ser levantado usando docker, para ello primero debemos de instalar las dependencias usando el comando `npm install`:

```
docker compose -f .docker/compose.yaml run node npm install
```

- Después de instalar las dependencias debemos levantar el contendor, el cual ya ejecutará de manera interna el comando `npm run dev`:

```
docker compose -f .docker/compose.yaml up -d
```
