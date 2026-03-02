# Térbol Landing - Sitio Web

Landing page institucional de **Térbol** y **Térbol Inspira**, desarrollada con Astro.

## 🚀 Estructura del Proyecto

```text
/
├── public/                          # Archivos públicos estáticos
│   ├── apple-touch-icon.png         # Icono para dispositivos Apple
│   ├── favicon.svg                  # Favicon del sitio
│   ├── favicon.ico                  # Favicon legacy
│   ├── heroimg.png                  # Imagen principal del hero
│   ├── site.webmanifest             # Manifiesto PWA
│   └── web-app-manifest-*.png       # Iconos PWA
│
├── src/
│   ├── assets/                       # Recursos procesados por Astro
│   │   ├── astro.svg                # Logo SVG de ejemplo
│   │   ├── background.svg           # Fondo SVG
│   │   ├── logo.svg                 # Logo principal
│   │   ├── fonts/                   # Fuentes personalizadas
│   │   │   ├── Roboto/             # Familia Roboto (Regular, Bold, etc.)
│   │   │   └── Roboto_Mono/        # Familia Roboto Mono
│   │   └── images/                  # Imágenes del proyecto
│   │       ├── b1.png               # Imágenes de banner
│   │       ├── f1.png, f2.png, f3   # Imágenes de features
│   │       ├── heroimg.png          # Imagen hero
│   │       ├── m-*.jpg              # Imágenes varias
│   │       ├── m*.png               # Más imágenes
│   │       └── product*.png         # Imágenes de productos
│   │
│   ├── components/                   # Componentes reutilizables
│   │   ├── common/                  # Componentes comunes
│   │   │   ├── Button.astro        # Botón polimórfico (a/button)
│   │   │   ├── Capsule.astro       # Cápsula decorativa
│   │   │   ├── FeatureCard.astro   # Tarjeta de característica
│   │   │   ├── Footer.astro        # Pie de página
│   │   │   ├── Navbar.astro        # Barra de navegación
│   │   │   ├── ProductCard.astro   # Tarjeta de producto
│   │   │   └── Step.astro          # Paso/Step
│   │   │
│   │   ├── icons/                   # Iconos SVG
│   │   │   ├── CircleCheck.astro   # Icono de check
│   │   │   ├── IconPassion.astro  # Icono de pasión
│   │   │   ├── IconPurpose.astro  # Icono de propósito
│   │   │   ├── IconQuality.astro  # Icono de calidad
│   │   │   └── IconRespect.astro  # Icono de respeto
│   │   │
│   │   └── landing/                 # Componentes de la landing
│   │       ├── About.astro          # Sección "Quiénes somos"
│   │       ├── Banner.astro        # Banner promocional
│   │       ├── Features.astro      # Sección de características
│   │       ├── Hero.astro           # Sección hero principal
│   │       ├── OurModel.astro      # Sección del modelo de negocio
│   │       └── Products.astro      # Sección de productos
│   │
│   ├── layouts/                     # Plantillas de página
│   │   └── Layout.astro            # Layout base HTML
│   │
│   ├── pages/                       # Páginas del sitio
│   │   └── index.astro             # Página principal
│   │
│   └── styles/                      # Estilos globales
│       ├── fonts.css               # Definiciones de fuentes
│       └── global.css              # Variables y estilos globales
│
├── astro.config.mjs                # Configuración de Astro
├── package.json                    # Dependencias y scripts
├── tsconfig.json                   # Configuración de TypeScript
└── README.md                       # Este archivo
```

## 🧞 Comandos

Todos los comandos se ejecutan desde la raíz del proyecto:

| Comando | Acción |
| :------ | :----- |
| `npm install` | Instala las dependencias |
| `npm run dev` | Inicia el servidor de desarrollo en `localhost:4321` |
| `npm run build` | Construye el sitio para producción en `./dist/` |
| `npm run preview` | Previsualiza el build localmente antes de desplegar |
| `npm run astro check` | Verifica tipos y errores |

## 📦 Dependencias

- **Astro** - Framework web moderno
- **TypeScript** - Tipado estático

## 🎨 Sistema de Diseño

### Colores

```css
--color-orange    /* Naranja principal */
--color-black     /* Negro */
--color-white     /* Blanco */
--color-soft-gray /* Gris suave */
--color-light-gray/* Gris claro */
--color-dark-gray /* Gris oscuro */
```

### Fuentes

- **Roboto** - Fuente principal (Regular, Medium, Bold, etc.)
- **Roboto Mono** - Fuente monoespaciada

### Componentes Reutilizables

#### Button
Botón polimórfico que renderiza `<a>` si tiene `href`, o `<button>` si no lo tiene.

```astro
<Button variant="primary" size="md" href="/pagina">Texto</Button>
```

**Variantes:** `primary`, `secondary`, `terciary`, `outline`, `ghost`  
**Tamaños:** `sm`, `md`, `lg`

#### FeatureCard
Tarjeta para mostrar características con icono.

```astro
<FeatureCard title="Título" description="Descripción">
  <Icon slot="icon" />
</FeatureCard>
```

## 📱 Responsive Breakpoints

- **Desktop:** > 1200px
- **Tablet:** 768px - 1200px  
- **Mobile:** < 768px

---

**Térbol Landing** - Desarrollado con Astro ⚡️
