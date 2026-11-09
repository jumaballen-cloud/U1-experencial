# Cookie Game

Una web para descubrir videojuegos y guardar tus favoritos. Desarrollada con React, Vite, React Router y Bootstrap. Conserva los colores y las imágenes locales de la landing original.

# Ejecutar

Instala Node.js 22.12 o superior. Abre una terminal en `cookie-game`:

```bash
npm ci
npm run dev
```

Abre la dirección que muestra Vite. Para compilar y revisar la versión de producción:

```bash
npm run build
npm run preview
```

# Rutas

`BrowserRouter` está en `src/main.jsx`. Las rutas se declaran directamente con `Routes` y `Route` en `src/App.jsx`. `Link` permite cambiar de vista y `NavLink` resalta la opción actual. `useParams` obtiene el identificador del juego en la vista de detalle.

Al publicar, el servidor debe redirigir las rutas de la aplicación a `index.html` para que los enlaces directos funcionen. Vite ya lo hace al desarrollar. No abrir `index.html` con doble clic: esta versión utiliza rutas y necesita el servidor de desarrollo o un alojamiento configurado para una SPA. Se retiró la antigua vista previa estática porque correspondía a la landing sin rutas.

# estructura

- `src/App.jsx`: rutas, estado de favoritos y función para agregar o quitar.
- `src/main.jsx`: inicio de React, BrowserRouter y estilos.
- `src/data/juegos.js`: datos e identificadores estables de los juegos.
- `src/pages/`: Inicio, Catalogo, DetalleJuego, Favoritos y NoEncontrado.
- `src/components/`: elementos reutilizables de la interfaz.
- `src/components/Juegos.jsx`: lista de tarjetas.
- `src/components/JuegoCard.jsx`: tarjeta con enlace al detalle y botón de favoritos.
- `src/components/BotonFavorito.jsx`: botón compartido por tarjetas y detalle.
- `src/assets/`: imágenes locales.
- `src/styles.css`: colores, tarjetas y adaptación a pantallas pequeñas.



Referencia: https://reactrouter.com/start/declarative/routing
