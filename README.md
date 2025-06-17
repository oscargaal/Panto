# 🛋️ Panto - Muebles Minimalistas y Modernos

Bienvenido al repositorio de Panto, una elegante landing page diseñada para una tienda de muebles que se especializa en diseños minimalistas y modernos. Este proyecto destaca la simplicidad, la elegancia y una excelente experiencia de usuario a través de un diseño responsivo y cuidadosamente elaborado.

## 🚀 Despliegue

La página está desplegada y accesible a través de Netlify:

[Ver Panto en Netlify](https://panto-oscargaal.netlify.app/)

## ✨ Características Principales

- **Diseño Moderno y Minimalista**: Interfaz limpia y atractiva que refleja la estética de los productos de mobiliario.
- **Diseño Responsivo**: Adaptado para ofrecer una experiencia óptima en una amplia gama de dispositivos, desde móviles hasta desktops.
  - Uso extensivo de clases `md:` y `lg:` de Tailwind CSS para una adaptación fluida.
- **Navegación Intuitiva**:
  - Barra de navegación superior con enlaces de categoría (`Furniture`, `Shop`, `About us`, `Contact`).
  - Icono de menú para dispositivos móviles.
  - Icono de carrito de compras.
- **Sección de Venta de Productos**:
  - Categorías de productos (`Chair`, `Beds`, `Sofa`, `Lamp`) con selección interactiva (aunque la interactividad real puede requerir JS).
  - Muestra de los productos más vendidos con detalles como nombre, precio y calificación por estrellas.
  - Navegación entre productos con flechas (ocultas en móvil).
- **Sección "Why Choosing Us"**: Destaca las ventajas de la empresa (instalaciones de lujo, precios asequibles, variedad de opciones).
- **Secciones de Experiencia y Materiales**: Contenido que subraya la calidad y profesionalidad en el diseño y fabricación de los muebles.
- **Testimonios de Clientes**: Sección dedicada a mostrar opiniones y reseñas de clientes.
- **Barra de Búsqueda Interactiva**: Facilita la búsqueda de productos.
- **Marcadores Interactivos en Portada**: Puntos de interés visual en la imagen principal (funcionalidad base en HTML/CSS, puede expandirse con JS).
- **Animaciones y Transiciones Suaves**:
  - Transiciones de color y escala en los enlaces de navegación al pasar el ratón (`:hover`).
  - Implementación de CSS puro para transiciones en `a:hover`.

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica de la página web.
- **Tailwind CSS**: Framework de CSS para un desarrollo rápido y un diseño altamente personalizable y responsivo.
  - Se utiliza un flujo de trabajo con `input.css` y `output.css` para la compilación de estilos.
- **CSS Puro**: Pequeñas adiciones de estilos personalizados para transiciones específicas de `hover` no cubiertas directamente por las utilidades de Tailwind (ej. `a:hover`).

## ⚙️ Configuración del Proyecto

Este proyecto es una landing page estática construida con HTML y estilizada con Tailwind CSS.

### `package.json`

El archivo `package.json` incluye scripts para el desarrollo y la compilación de Tailwind CSS:

```json
{
  "name": "dom-project",
  "version": "1.0.0",
  "author": "Germinal Camps for CodeOp",
  "license": "MIT",
  "scripts": {
    "start": "npx @tailwindcss/cli -i ./input.css -o ./output.css --watch",
    "build": "npx @tailwindcss/cli -i ./input.css -o ./output.css --minify"
  },
  "devDependencies": {
    "prettier-plugin-tailwindcss": "^0.6.11",
    "@tailwindcss/cli": "^4.0.15",
    "tailwindcss": "^4.1.5"
  }
}
```

- `npm run start`: Inicia el modo de observación de Tailwind CSS, recompilando `output.css` cada vez que se guarda `input.css` o los archivos HTML referenciados. Ideal para desarrollo local.
- `npm run build`: Compila y minifica el CSS final desde `input.css` a `output.css`. Este script es crucial para el despliegue en entornos de producción como Netlify.

### 📁 Estructura de Archivos

```
├── public/                 # (O la raíz del proyecto si tus imágenes/sonidos están allí)
│   ├── img/
│   │   ├── portada.png
│   │   ├── flechita_abajo.svg
│   │   ├── carrito_compra.png
│   │   └── ... (y todas las demás imágenes usadas)
│   └── sound/              # (Si hubiera algún archivo de sonido, aunque no se usa en el HTML proporcionado)
├── input.css               # Archivo CSS fuente con directivas de Tailwind
├── output.css              # Archivo CSS compilado por Tailwind
├── index.html              # Página principal de la landing page
├── package.json            # Configuración del proyecto y scripts
├── tailwind.config.js      # Configuración de Tailwind CSS
└── README.md               # Este archivo
```

## 🚀 Cómo Ejecutar el Proyecto Localmente

Clona el repositorio:

```bash
git clone https://github.com/oscargaal/Panto
cd https://github.com/oscargaal/Panto
```

Instala las dependencias:

```bash
npm install
```

Inicia el modo de desarrollo de Tailwind CSS:

```bash
npm run tailwind
```

Esto generará `output.css` y lo mantendrá actualizado mientras trabajas.

Abre `index.html` directamente en tu navegador (o usa una extensión de "Live Server" para un mejor desarrollo).

## 📄 Licencia

Este proyecto está bajo la licencia **MIT**, como se especifica en el `package.json`.

## ✉️ Contacto

Puedes contactarme a través de:

* **GitHub:** [oscargaal](https://github.com/oscargaal)
* **LinkedIn:** [Oscar García](https://www.linkedin.com/in/oscar-garc%C3%ADa-b4a755308/)
