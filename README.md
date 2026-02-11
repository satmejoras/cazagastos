# 💰 Mi Economía - PWA

Gestor personal de gastos que funciona 100% offline en tu móvil.

## 📱 Instalación en iPhone/iPad (iOS)

### Opción 1: Hosting en GitHub Pages (RECOMENDADO)

1. **Sube los archivos a GitHub:**
   - Crea un repositorio nuevo en GitHub
   - Sube todos los archivos de esta carpeta
   - Ve a Settings → Pages
   - Source: "Deploy from a branch" → "main" → "/ (root)"
   - Guarda y espera 1-2 minutos

2. **Instala en tu iPhone:**
   - Abre Safari en tu iPhone
   - Ve a la URL de GitHub Pages (ej: `https://tu-usuario.github.io/mi-economia`)
   - Toca el botón "Compartir" 📤
   - Toca "Añadir a pantalla de inicio"
   - ¡Listo! Ya tienes el icono en tu home screen

### Opción 2: Hosting en Netlify (MÁS RÁPIDO)

1. **Sube a Netlify:**
   - Ve a [netlify.com](https://netlify.com)
   - Arrastra la carpeta completa a Netlify Drop
   - Te da una URL automática

2. **Instala igual que arriba** usando Safari

### Opción 3: Hosting local con ngrok (TEMPORAL)

```bash
# En tu ordenador
cd carpeta-de-la-pwa
python3 -m http.server 8000

# En otra terminal
ngrok http 8000
# Copia la URL https:// que te da ngrok
# Ábrela en Safari del iPhone
# Instala como PWA
```

## 📱 Instalación en Android

1. Abre Chrome en Android
2. Ve a la URL de tu PWA
3. Toca el menú (⋮)
4. Toca "Añadir a pantalla de inicio"
5. ¡Instalado!

## ✨ Características PWA

✅ **Funciona 100% offline** (después de la primera visita)
✅ **localStorage funciona** (tus datos se guardan en el móvil)
✅ **Exportar CSV funciona** (descarga directa)
✅ **Se ve como app nativa** (sin barra del navegador)
✅ **Icono en home screen**

## 📁 Archivos incluidos

```
index.html          → Tu gestor de gastos
manifest.json       → Configuración PWA
sw.js              → Service Worker (funcionalidad offline)
icon-192.png       → Icono 192x192
icon-512.png       → Icono 512x512
README.md          → Este archivo
```

## 🔧 Personalización

### Cambiar colores
Edita `manifest.json`:
```json
"background_color": "#f5f5f7",  ← Color de fondo
"theme_color": "#007aff"        ← Color del tema
```

### Cambiar nombre
Edita `manifest.json`:
```json
"name": "Mi Economía",      ← Nombre completo
"short_name": "Economía"    ← Nombre corto (debajo del icono)
```

### Cambiar icono
Reemplaza `icon-192.png` y `icon-512.png` con tus propios iconos.

## 🐛 Troubleshooting

**¿No se instala en iOS?**
- Asegúrate de usar **Safari** (no Chrome)
- La URL debe ser **HTTPS** (no HTTP)
- GitHub Pages y Netlify ya son HTTPS automáticamente

**¿No funciona offline?**
- Abre la app una vez con internet
- Cierra Safari completamente
- Prueba de nuevo

**¿Los datos se borran?**
- No, localStorage persiste
- Solo se borran si desinstalas la app o limpias datos del navegador

## 📤 Exportar datos

El botón "Exportar CSV" descarga directamente en tu móvil.
En iOS: Los archivos van a la carpeta "Archivos" → "Descargas"

## 🎯 Siguientes pasos

1. Hostea en GitHub Pages o Netlify
2. Instala en tu iPhone
3. Úsala como cualquier app nativa
4. Tus datos están 100% en tu móvil (privados)

---

**¿Dudas?** Esta PWA es tu HTML convertido para funcionar en móvil sin App Store 🚀
