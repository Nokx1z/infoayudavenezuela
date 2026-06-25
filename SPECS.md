# 📋 Especificaciones Técnicas (specs.md) - Plataforma de Centros de Acopio Venezuela

Este proyecto es una plataforma web de código abierto diseñada para centralizar, verificar y mapear los centros de acopio activos en Venezuela. Está optimizada para cargar con extrema rapidez en conexiones móviles de baja velocidad (2G/3G/4G).

---

## 1. Arquitectura Tecnológica

* **Frontend/Backend:** Astro (Configurado en modo SSR/Híbrido para ocultar credenciales y acelerar cargas).
* **Base de Datos:** MongoDB (NoSQL) para un manejo flexible de documentos JSON sin migraciones rígidas.
* **Driver de Conexión:** Driver oficial de Node.js `mongodb`.
* **Estilos:** Tailwind CSS (Para una interfaz minimalista, ligera y responsiva).

---

## 2. Configuración del Servidor (Astro SSR)

Para poder ejecutar consultas a MongoDB de forma segura en el lado del servidor, el proyecto opera bajo arquitectura SSR.

### Configuración del Adaptador (`astro.config.mjs`)
```javascript
import { defineConfig } from 'astro/config';
import vercel from '@astrojs/vercel/serverless'; // O el adaptador correspondiente de hosting

export default defineConfig({
  output: 'server', // Habilita el entorno de servidor en todo el proyecto
  adapter: vercel(),
});