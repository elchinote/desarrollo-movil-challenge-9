## Challenge 9 del curso de Desarrollo Móvil de Coderhouse

Para poder resolver este challenge seguir los siguientes pasos

1. Hacer un **fork** este repositorio
1. Una vez hecho el **fork**, hacer un clon copiando la URL (en el botón verde) y corriendo `git clone <URL>` en la consola
1. Una vez clonado, moverse dentro de la carpeta del proyecto y correr `npm install` (o `yarn`) para instalar las dependencias necesarias
1. Hacer un **nuevo branch** con tu nombre y apellido para identificarte (ej. `git checkout -b gonzalo-aguirre`)
1. Correr el proyecto usando `expo start`
1. Resolver el enunciado, **haciendo un nuevo commit al resolver cada parte**
1. Hacer un **push** del nuevo branch
1. Desde **github.com** crear un nuevo **pull request** desde ese branch hacia master

### Enunciado

### Configuración Previa

1. Cambiar el `SPOTIFY_CLIENT_ID` con su `clientId`
1. Agregar la nueva `redirectUrl` en la configuración de Spotify 
> Debería ser `https://auth.expo.io/@<TU_USERNAME>/desarrollo-movil-challenge-9`, pero podés verificarlo haciendo un `console.warn('Mi url', redirectUrl)` debajo de la llamada a `AuthSession.getRedirectUrl()` en el archivo `spotify-api-client.js`

#### Integrando Firebase
1. Instalar el SDK de Firebase como dependencia
    > `yarn add firebase` o `npm install firebase`
1. Crear un archivo llamado `firebase.js` y dentro del mismo copiar el snippet que nos da Firebase con la inicialización del mismo

#### Integrando Firestore
1. Integrar **Firestore** importandolo `import 'firebase/firestore'` en nuestro archivo `firebase.js`
1. Seguir el **Get Started** desde el paso **Initialize Cloud Firestore** (https://firebase.google.com/docs/firestore/quickstart?authuser=0)
1. Probar de insertar data y corroborar que haya funcionado en el dashboard

#### Peristiendo datos en Firestore
1. Definir una estructura de cómo guardar los artistas favoritos
1. Una vez definida esa estructura, persistir los favoritos al tocar el botón de _favorito_

#### Identificando los fans
Para poder identificar cuáles son los fans de cada artista, tendremos que agregar autenticación con Firebase.
Vamos a integrar Facebook, para el que Expo provee un buen componente.

1. Seguir la guía de Expo de cómo integrar Facebook login
> (https://docs.expo.io/versions/latest/sdk/facebook)
1. TBD

