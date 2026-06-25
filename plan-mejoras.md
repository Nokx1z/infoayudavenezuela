# Plan de Mejoras

## Tareas Pendientes para Próximas Iteraciones

### 1. Migración a SSR + MongoDB (según SPECS.md)
- [ ] Cambiar `output: 'static'` a `output: 'server'` en `astro.config.mjs`
- [ ] Agregar adaptador de hosting (Vercel / Netlify)
- [ ] Configurar conexión a MongoDB con driver oficial `mongodb`
- [ ] Migrar datos de `acopio.json` y `numerosemergencia.json` a MongoDB
- [ ] Crear API endpoints para consultas desde el servidor
- [ ] Implementar autenticación para moderación de datos

### 2. Base de Datos
- [ ] Diseñar esquema de colecciones en MongoDB
- [ ] Crear seed scripts para carga inicial de datos
- [ ] Implementar sistema de moderación/validación de nuevos centros
- [ ] Historial de cambios (log de actualizaciones por centro)

### 3. Funcionalidades
- [ ] Mapa interactivo con ubicación de centros de acopio
- [ ] Filtros avanzados (por insumo aceptado, por necesidad urgente)
- [ ] Sistema de reportes: usuarios pueden reportar centros saturados/cerrados
- [ ] Notificaciones de cambios en centros cercanos
- [ ] Modo offline / PWA para consulta sin conexión
- [ ] Compartir centro por WhatsApp / redes sociales

### 4. Performance (Cero Desperdicio de Datos)
- [ ] Evaluar si Tailwind CSS es necesario o conviene seguir con CSS nativo
- [ ] Auditoría de peso de página con Lighthouse
- [ ] Optimizar imágenes de banderas (SVG a inline o sprite)
- [ ] Implementar lazy loading estratégico

### 5. Estilos y UX
- [ ] Revisar paleta de colores definitiva
- [ ] Mejorar feedback visual en acciones (toast/notificaciones)
- [ ] Animaciones de carga/transición sutiles
- [ ] Modo alto contraste para accesibilidad

### 6. Infraestructura
- [ ] Configurar CI/CD para despliegue automático
- [ ] Dominio personalizado
- [ ] SSL/HTTPS
- [ ] Monitoreo de disponibilidad
