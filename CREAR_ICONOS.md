# 🎨 Cómo Crear los Iconos para la PWA

La aplicación necesita dos iconos para funcionar como PWA instalable:

## 📏 Especificaciones

- **icon-192.png**: 192x192 píxeles
- **icon-512.png**: 512x512 píxeles

Ambos deben ser:
- Formato PNG con fondo transparente u opaco
- Diseño simple y reconocible
- Preferiblemente cuadrados con esquinas redondeadas

## 🛠️ Opciones para Crear los Iconos

### Opción 1: Usar un Generador Online (Más Fácil)

1. Ve a uno de estos sitios:
   - https://www.favicon-generator.org/
   - https://realfavicongenerator.net/
   - https://favicon.io/

2. Sube una imagen base (puede ser el emoji 🕵️ como captura de pantalla)

3. Genera los iconos en los tamaños necesarios

4. Descarga los archivos y guárdalos como:
   - `icon-192.png`
   - `icon-512.png`

### Opción 2: Diseñar con Canva (Gratis)

1. Ve a [Canva](https://www.canva.com/)
2. Crea un diseño de 512x512 px
3. Usa el emoji 🕵️ o diseña tu propio icono
4. Exporta como PNG
5. Redimensiona a 192x192 para el icono pequeño

### Opción 3: Usar Figma o Adobe Illustrator

1. Crea un canvas de 512x512 px
2. Diseña el icono (sugerencia: emoji detective 🕵️ con fondo de color)
3. Exporta en dos tamaños: 192x192 y 512x512

### Opción 4: Con GIMP o Photoshop

1. Crea un nuevo archivo de 512x512 px
2. Añade el emoji 🕵️ o crea un diseño personalizado
3. Guarda una copia como `icon-512.png`
4. Redimensiona la imagen a 192x192 px
5. Guarda como `icon-192.png`

## 🎨 Sugerencias de Diseño

**Idea Simple:**
- Fondo gradiente (morado/azul: #6366f1 a #4f46e5)
- Emoji detective 🕵️ centrado en blanco
- Texto "Impostor" debajo (opcional)

**Idea Minimalista:**
- Fondo sólido color primario (#6366f1)
- Letra "I" grande y bold en blanco
- Círculo o borde redondeado

**Idea Temática:**
- Silueta de detective con sombrero
- Lupa con signo de interrogación
- Máscara de impostor

## 📁 Ubicación Final

Una vez creados, coloca los archivos en la raíz del proyecto:

```
impostor-game/
├── icon-192.png    ← Aquí
├── icon-512.png    ← Aquí
├── index.html
├── manifest.json
└── ...
```

## ⚠️ Nota

Si no quieres crear iconos ahora, la aplicación **funcionará perfectamente** sin ellos. Solo afectará:
- El icono al instalar la PWA (usará uno genérico)
- La apariencia en la pantalla de inicio del móvil

Puedes añadirlos más tarde sin problemas.

## ✅ Verificación

Para verificar que los iconos funcionan:

1. Abre las DevTools del navegador (F12)
2. Ve a "Application" → "Manifest"
3. Verifica que los iconos aparezcan correctamente
4. Si hay errores, revisa las rutas en `manifest.json`

---

**¡Listo! Con los iconos tu PWA se verá profesional en todos los dispositivos.** 🎉
