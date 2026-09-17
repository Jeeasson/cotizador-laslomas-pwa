# 🏗️ LAS LOMAS — Cotizador Pro & PWA de Materiales

**Cotizador rápido, moderno y 100% offline para distribución de materiales de acero y construcción.**
Desarrollado como una **Progressive Web App (PWA)** de alto rendimiento, optimizado para celulares, tablets y ordenadores.

---

## 🚀 Características Principales

- ⚡ **Velocidad y Fluidez Ultra-Rápida**: Renderizado optimizado por lotes (chunking), filtrado debounceado con `requestAnimationFrame`, y aceleración por GPU.
- 📱 **PWA Completa & 100% Offline**: Funciona sin conexión a internet gracias al Service Worker dedicado (`sw.js`). Se puede instalar directamente en la pantalla de inicio de Android, iOS o Windows/Mac.
- 📄 **Exportación a PDF Vectorial (Texto Real)**: Generador PDF 1.4 integrado sin dependencias externas. Documentos nítidos con encabezados, logo oficial, cálculo de fletes y textos seleccionables y buscables.
- 🖼️ **Exportación de Proforma en Imagen (1080px)**: Diseños verticales de alta definición listos para compartir al instante por WhatsApp o correo.
- 🧮 **Calculadora de Fierros Corrugados por Gestos**: Control táctil intuitivo donde deslizar suma o resta toneladas por diámetro.
- 📊 **Gestión Integral**: Catálogo de productos con importación/exportación masiva en Excel (XLSX) y CSV, historial de cotizaciones, estadísticas, directorio de clientes y seguimiento de estados.
- 🔒 **Seguridad y Privacidad**: Bloqueo por código PIN, modo privacidad para ocultar montos y datos guardados exclusivamente en el almacenamiento local del dispositivo.
- 🎨 **4 Temas Visuales**: Verde Corporativo, Claro, Oscuro OLED y Azul Técnico.

---

## 📂 Estructura de Árbol del Proyecto (PWA Architecture)

```
KOtizaDor/
├── index.html                   # Aplicación principal optimizada y auditada
├── manifest.webmanifest         # Manifiesto PWA estándar (W3C)
├── manifest.json                # Manifiesto compatible
├── sw.js                        # Service Worker para caché y modo offline
├── icons/                       # Iconos PWA y de plataforma
│   ├── icon-192.png             # Icono estándar (192x192)
│   ├── icon-512.png             # Icono alta resolución (512x512)
│   ├── icon-maskable-192.png    # Icono adaptable Android (192x192)
│   ├── icon-maskable-512.png    # Icono adaptable Android (512x512)
│   ├── apple-touch-icon.png     # Icono para dispositivos Apple iOS (180x180)
│   └── favicon.png              # Favicon para navegadores web
├── .gitignore                   # Exclusiones de Git
└── README.md                    # Documentación del proyecto
```

---

## 📲 Cómo Instalar la PWA

### En Android (Chrome / Edge / Samsung Internet):
1. Abre la URL en tu navegador.
2. Toca el menú de tres puntos (⋮) o el botón "Añadir a pantalla de inicio" / "Instalar aplicación".
3. La aplicación se instalará como una app nativa en tu teléfono.

### En iPhone / iPad (Safari):
1. Abre la URL en Safari.
2. Toca el botón **Compartir** (cuadrado con flecha hacia arriba).
3. Selecciona **"Añadir a la pantalla de inicio"**.

### En Computadora (Chrome / Edge):
1. Haz clic en el icono de instalación en el lado derecho de la barra de direcciones (o en el menú de Ajustes → Instalar PWA).

---

## 🛠️ Tecnologías Utilizadas

- **HTML5 / CSS3 Avanzado**: Variables CSS, diseño responsivo, temas dinámicos, glassmorphism con aceleración por hardware.
- **JavaScript Vanilla Moderno**: Sin frameworks pesados ni dependencias externas, asegurando carga instantánea y máxima compatibilidad.
- **Web App Manifest & Service Worker API**: Caché inteligente de recursos y capacidad de funcionamiento sin internet.
- **Canvas API**: Renderizado gráfico para proformas en imagen.
- **Motor PDF 1.4 Propio**: Generación directa de flujo binario PDF sin librerías de terceros.
