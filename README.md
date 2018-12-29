# Hosting with firebase

Con este tutorial podra desplegar una aplicación react usando Firebase. 

Para iniciar debe instalar las herramientas CLI que provee Firebase
> npm install -g firebase-tools

Luego de la instalación debe hacer la autenticación con su cuenta Gmail 
> firebase login

Al finalizar la autenticación debe ir a la raiz de su proyecto mediante la terminal de comandos CMD e iniciar un proyecto de Firebase
> firebase init

Cuando inicialice el proyecto saldrán algunas opciones a seleccionar, la primera debe ser acepatada
> Are you ready to proceed? YES

Luego saldran nuevas opciones y debe seleccionar unicamente la de Hosting 
> (*) Hosting: Configure and deploy Firebase Hosting sites

(crear un proyecto en el dashboard de Firebase para que aparezca el proyecto en la siguiente pregunta)

> ? Select a default Firebase project for this directoy: 

Aquí debe seleccionar el proyecto que creo en Firebase 

Cuando crea un proyecto de React se crea un directorio llamado Public y la siguiente pregunta define el directorio publico a usar, por esta razón se debe dejar por defecto este directorio

Al finalizar esta configuración se crean dos nuevos ficheros:
  > firebase.json
  
  > .firebaserc (Aquí se almacena la configuración que se usa para el despliegue de la aplicación)

Finalmente usamos el siguiente comando para hacer el despliegue  
 
 > firebase deploy 

Si no aparece la aplicación en la dirección de Hosting intente correr el siguiente comando antes de hacer un nuevo deploy

 > npm run build

y de nuevo 

 > firebase deploy 
