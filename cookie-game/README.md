
Cookie Game

Cookie Game es una aplicación web desarrollada para descubrir videojuegos, explorar diferentes categorías y administrar una lista de favoritos. El proyecto fue construido con React, Vite, React Router y Bootstrap, conservando los colores e imágenes de la versión original de la landing page.

Ejecución del proyecto

Para ejecutar la aplicación es necesario contar con Node.js versión 22.12 o superior. Una vez ubicado en la carpeta cookie-game, se deben instalar las dependencias mediante el comando npm ci y luego iniciar el entorno de desarrollo con npm run dev. Posteriormente, se accede desde el navegador a la dirección local generada por Vite.

Para generar la versión de producción se utiliza el comando npm run build y para visualizar el resultado compilado se ejecuta npm run preview.

Rutas y navegación

La navegación de la aplicación se implementa mediante React Router. BrowserRouter se encuentra configurado en src/main.jsx y las rutas son definidas en src/App.jsx mediante Routes y Route. Los componentes Link y NavLink permiten la navegación entre páginas, mientras que useParams se utiliza para obtener el identificador de cada videojuego en la vista de detalle.

Al desplegar la aplicación en producción, el servidor debe redirigir todas las solicitudes hacia index.html para garantizar el correcto funcionamiento de la aplicación de página única (SPA). No se recomienda abrir el archivo index.html directamente desde el sistema de archivos porque la aplicación requiere un servidor web para gestionar las rutas.

Estructura del proyecto

src/App.jsx contiene la configuración de rutas, el estado de favoritos y las funciones para agregar o eliminar 
