# ⚡ PriceSync 2.1

**Sincronizador de stock y precios** entre tu software de gestión y Tienda Nube.

## 🚀 Demo en vivo

👉 **[Abrir PriceSync 2.1](https://TU_USUARIO.github.io/pricesync2.1/)**

> Reemplazá `TU_USUARIO` con tu nombre de usuario de GitHub después de publicar.

## ¿Qué hace?

PriceSync toma el archivo Excel/CSV de tu software de gestión de juguetería y el CSV exportado de Tienda Nube, los cruza automáticamente y genera un CSV actualizado listo para importar con:

- ✅ **Stock sincronizado** (con resta configurable, ej: stock gestión - 1)
- ✅ **Precios actualizados** desde Lista 2 del sistema de gestión
- ✅ **Códigos de barras completados** en productos que no los tenían en Tienda Nube

## Cómo funciona

### Paso 1: Subir archivos
- Archivo Excel (.xlsx/.xls) o CSV de tu software de gestión
- Archivo CSV descargado de Tienda Nube

### Paso 2: Mapear columnas
- Auto-detecta columnas de código de barras, nombre, stock y precio
- Configurá cuánto restar al stock (por defecto: 1)

### Paso 3: Revisar y descargar
- Vista previa de todas las coincidencias
- Match por **código de barras** (exacto) y por **nombre** (fuzzy matching)
- Filtros clickeables para revisar coincidencias dudosas
- Editar stock y precio individualmente
- Descargar CSV listo para Tienda Nube

## Características

- 🔍 **Matching inteligente**: Primero por código de barras, luego por nombre con algoritmo de similitud
- 📋 **Copia de códigos de barras**: Completa automáticamente los códigos faltantes en Tienda Nube
- 💰 **Sincronización de precios**: Mapea Precio Lista 2 del gestión al campo de precio de TN
- 🔤 **Soporte de acentos**: Lee correctamente archivos con ñ, acentos y caracteres especiales (UTF-8 y Windows-1252)
- 🔒 **100% local**: Tus datos nunca salen de tu navegador. No hay servidor, no se sube nada a la nube.

## Tecnologías

- React 18 (via CDN)
- SheetJS para lectura de Excel
- Babel standalone para JSX
- GitHub Pages para hosting

## Instalación local

No necesitás instalar nada. Simplemente abrí `index.html` en tu navegador.

## Publicar en GitHub Pages

1. Creá un repositorio en GitHub (ej: `pricesync2.1`)
2. Subí los archivos
3. Andá a **Settings → Pages → Source: Deploy from branch → main → / (root)**
4. Tu app estará en `https://tu-usuario.github.io/pricesync2.1/`

---

Hecho con ⚡ para sincronizar jugueterías con Tienda Nube.
