# Prueba Técnica Caypre

Aplicación web desarrollada como prueba técnica para **Caypre**. Consiste en un catálogo de productos (monitores) construido con **Nuxt.js** y **Vuetify**, donde se muestran los datos de artículos en formato tabla y se transforman visualmente en fichas de producto.

## Tech Stack

| Tecnología   | Versión | Propósito                          |
| ------------ | ------- | ---------------------------------- |
| **Nuxt.js**  | ^2.0.0  | Framework SSR/SPA sobre Vue.js     |
| **Vuetify**  | ^2.6.7  | Biblioteca de componentes UI (Material Design) |
| **Vuex**     | —       | Manejo de estado (integrado en Nuxt) |
| **SASS**     | ^1.22.9 | Preprocesador CSS para estilos     |
| **Node.js**  | —       | Entorno de ejecución               |

## Estructura del Proyecto

```
pruebateccaypre/
├── assets/
│   ├── README.md
│   └── style/
│       ├── app.styl
│       └── variables.styl
├── components/
│   └── README.md
├── layouts/
│   ├── default.vue          # Layout principal con v-app y footer
│   └── README.md
├── middleware/
│   └── README.md
├── pages/
│   ├── index.vue            # Página principal con tabla y fichas de producto
│   └── README.md
├── plugins/
│   └── README.md
├── static/
│   ├── favicon.ico
│   ├── v.png
│   └── README.md
├── store/
│   └── README.md            # Directorio preparado para Vuex store
├── nuxt.config.js           # Configuración de Nuxt y Vuetify
├── package.json
└── README.md
```

## Instalación y Configuración

### Requisitos previos

- **Node.js** (v12 o superior)
- **npm** (v6 o superior)

### Pasos

```bash
# 1. Clonar el repositorio
git clone https://github.com/sitokat/pruebateccaypre.git
cd pruebateccaypre

# 2. Instalar dependencias
npm install

# 3. Iniciar en modo desarrollo (con hot-reload)
npm run dev

# 4. Abrir en el navegador
# http://localhost:3000
```

### Compilación para producción

```bash
# Generar la build de producción
npm run build

# Iniciar el servidor en producción
npm start

# Generar sitio estático
npm run generate
```

## Características Implementadas

### Funcionalidades principales

- **Catálogo de productos** — Visualización de una tabla con datos de monitores (nombre, descripción corta, precio, URL de imagen).
- **Interfaz con Vuetify** — Componentes Material Design responsivos (`v-layout`, `v-card`, `v-data-table`, `v-footer`).
- **Configuración temática** — Tema claro/oscuro configurable mediante Vuetify theme en `nuxt.config.js`.
- **Estructura Nuxt modular** — Separación en páginas, layouts, componentes, store y assets.

### Extras planeados / en desarrollo

Los siguientes puntos forman parte de los requisitos extra de la prueba técnica y están disponibles para ser implementados:

- [ ] Conversión de tabla de datos a fichas de producto (tarjetas visuales)
- [ ] Paginación con parámetro en la URL (`?page=N`)
- [ ] Carrito de compra con botón "Comprar"
- [ ] Vista responsiva para móviles
- [ ] Backend con base de datos y dump SQL
- [ ] Middleware de autenticación con roles (admin / usuario)
- [ ] Panel de administración para gestionar productos
- [ ] Sesión persistente mediante cookies
- [ ] Despliegue en servidor web público

## Scripts Disponibles

| Comando             | Descripción                              |
| ------------------- | ---------------------------------------- |
| `npm run dev`       | Inicia servidor de desarrollo con recarga en caliente |
| `npm run build`     | Compila la aplicación para producción    |
| `npm start`         | Inicia el servidor en modo producción    |
| `npm run generate`  | Genera el sitio como archivos estáticos  |

## Licencia

Proyecto privado — Prueba técnica para proceso de selección.

---

Desarrollado con ❤️ usando [Nuxt.js](https://nuxtjs.org) y [Vuetify](https://vuetifyjs.com).
