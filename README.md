# Keep Aligned Landing Page

Landing page para [keepaligned.com](https://keepaligned.com) - La app para seguir tu tratamiento de ortodoncia invisible.

## Stack

- **[Astro](https://astro.build/)** - Framework para sitios estáticos ultra-rápidos
- **[Tailwind CSS v4](https://tailwindcss.com/)** - Estilos con design tokens personalizados
- **[Netlify](https://netlify.com/)** - Hosting y deploy automático

## Desarrollo

```bash
# Instalar dependencias
npm install

# Servidor de desarrollo (http://localhost:4321)
npm run dev

# Build para producción
npm run build

# Preview del build
npm run preview
```

## Estructura

```
src/
├── components/
│   ├── Header.astro          # Navegación y logo
│   ├── Footer.astro          # Footer con links
│   ├── Hero.astro            # Sección principal con CTA
│   ├── Features.astro        # Grid de funcionalidades
│   ├── FeatureCard.astro     # Tarjeta de feature
│   ├── AppShowcase.astro     # Showcase con tabs interactivos
│   ├── ForOrthodontists.astro # Sección para profesionales
│   ├── FinalCTA.astro        # CTA final de descarga
│   ├── DownloadButtons.astro # Botones de App Store/Play Store
│   └── mockups/
│       ├── PhoneFrame.astro      # Marco de teléfono
│       ├── HomeScreenMockup.astro
│       ├── CalendarMockup.astro
│       ├── TimerMockup.astro
│       └── ProgressMockup.astro
├── layouts/
│   └── Layout.astro          # Layout base con meta tags
├── pages/
│   └── index.astro           # Página principal
└── styles/
    └── global.css            # Design system tokens
```

## Design System

Los tokens de diseño están definidos en `src/styles/global.css` usando Tailwind CSS v4 `@theme`:

- **Colores**: Brand blues, neutrals, success/warning/danger
- **Tipografía**: Plus Jakarta Sans
- **Espaciado y radios**: Consistentes con la app móvil

## Deploy

El sitio se despliega automáticamente en Netlify cuando se hace push a `main`.

Configuración en `netlify.toml`:
- Build command: `npm run build`
- Publish directory: `dist`

## Relacionado

- **[keep-aligned-mobile](https://github.com/agustinarone/keep-aligned-mobile)** - App móvil React Native/Expo
