# Centros de Acopio Venezuela

## Contexto

El **24 de junio de 2026**, dos sismos de magnitud **7.5 y 7.2** sacudieron la región central de Venezuela, afectando severamente a Caracas y los estados Miranda, La Guaira, Aragua y Carabobo. La emergencia generó una movilización civil masiva para la recolección de insumos, pero la información sobre centros de acopio activos circula de forma desorganizada en redes sociales.

Esta plataforma centraliza, verifica y organiza los centros de acopio habilitados por estado y ciudad, permitiendo a los ciudadanos encontrar rápidamente dónde llevar donaciones y consultar los números de emergencia activos.

## Filosofía de Diseño

- **Cero desperdicio de datos**: Sin librerías pesadas, sin JavaScript innecesario. Cada kilobyte cuenta para un usuario en una red móvil inestable.
- **Rapidez ante todo**: HTML estático generado en build, consulta inmediata sin esperar peticiones al servidor.
- **Información verificada**: Los datos se publican solo tras validación manual del equipo moderador.

## Stack Actual

| Capa | Tecnología |
|------|-----------|
| Framework | Astro (static output) |
| Datos | JSON plano embebido en build |
| Estilos | CSS nativo |
| Fuentes | Sistema nativo (sin Google Fonts) |
| Hosting | Estático (Vercel / Netlify / cualquier CDN) |

## Mejoras Planificadas

Ver `plan-mejoras.md` para el roadmap que incluye migración a SSR + MongoDB, mapa interactivo, modo offline/PWA y más.

## Licencia

Código abierto — construido por y para la comunidad venezolana.
