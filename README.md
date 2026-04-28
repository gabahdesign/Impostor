# 🕵️ Juego del Impostor

Una aplicación web progresiva (PWA) para jugar al clásico juego de deducción social del impostor. Desarrollada con HTML5, CSS3 y JavaScript vanilla sin dependencias externas.

## 🎮 Descripción

El Juego del Impostor es un juego de deducción social donde los jugadores deben identificar quién es el impostor entre ellos. Todos los jugadores civiles reciben la misma palabra secreta, mientras que el impostor no la conoce y debe intentar descubrirla sin revelar su identidad.

## ✨ Características

- **📱 Mobile-First**: Diseño optimizado para dispositivos móviles
- **🌓 Modo Oscuro**: Tema claro y oscuro
- **🌍 Multiidioma**: Soporte para Español, Inglés y Català
- **💾 PWA**: Instalable como aplicación nativa
- **🎯 11 Categorías**: Más de 2000 palabras en 11 categorías temáticas
- **🔞 Control Parental**: Categoría +18 con verificación de edad
- **👥 3-15+ Jugadores**: Soporta de 3 a 15+ jugadores
- **🎲 Impostores Variables**: Flexible - hasta (jugadores - 1) impostores
- **📊 Historial**: Seguimiento de eliminaciones y resultados
- **💾 Persistencia Local**: Configuración guardada automáticamente

## 🚀 Inicio Rápido

### Opción 1: Abrir Directamente

1. Descarga todos los archivos del proyecto
2. Abre `index.html` en tu navegador
3. ¡Comienza a jugar!

### Opción 2: Servidor Local (Recomendado para PWA)

Para aprovechar todas las características PWA, es recomendable usar un servidor local:

#### Usando Python 3:
```bash
python -m http.server 8000
```

#### Usando Node.js (http-server):
```bash
npx http-server
```

#### Usando PHP:
```bash
php -S localhost:8000
```

Luego accede a `http://localhost:8000` en tu navegador.

## 📖 Cómo Jugar

### 1. Configuración Inicial
**Añadir Jugadores**:
- Ve a la pestaña "Jugadores"
- Introduce el nombre de cada jugador
- Necesitas mínimo 3 jugadores

**Seleccionar Temas**:
- Ve a la pestaña "Configuración"
- Selecciona al menos un tema de las 11 categorías disponibles:
  - Alimentación (frutas, verduras, bebidas, postres...)
  - Animales (mamíferos, aves, acuáticos, insectos...)
  - Lugares del Mundo (ciudades, países, monumentos...)
  - Objetos Cotidianos (tecnología, hogar, herramientas...)
  - Personas y Roles (profesiones, oficios, personajes...)
  - Ocio y Cultura (deportes, música, cine, arte...)
  - Deportes (deportes olímpicos, extremos, acuáticos...)
  - Emociones y Estados (sentimientos, estados de ánimo...)
  - Acciones (verbos, actividades cotidianas...)
  - Características (colores, tamaños, texturas...)
  - Adultos (+18) (requiere verificación de edad)
- Puedes seleccionar múltiples categorías si lo deseas

**Configurar Impostores**:
- En la pestaña "Jugadores"
- Elige el número de impostores (desde 1 hasta total de jugadores - 1)
- O activa "Número aleatorio" para sorpresa

### 2. Comenzar Partida
Presiona "Comenzar Juego" en la pestaña Jugadores
El juego asignará roles aleatoriamente
Seleccionará un tema y palabra al azar

### 3. Revelación de Roles
Pasa el dispositivo al primer jugador
El jugador presiona "Ver mi Rol"
El jugador verá:
- Si es Civil: El tema y la palabra secreta
- Si es Impostor: Solo el tema, NO la palabra

El jugador presiona "Siguiente Jugador"
Repite hasta que todos vean su rol

### 4. Fase de Discusión
Los jugadores discuten sobre el tema
Los civiles intentan demostrar que conocen la palabra sin revelarla
El impostor intenta descubrir la palabra o confundir a los demás
No uses la app en esta fase, ¡solo hablad!

### 5. Votación
1. Ve a la pestaña "Votación"
2. Vota por el jugador que crees que es el impostor
3. El jugador eliminado se revela:
   - Si era impostor: ¡Se muestra!
   - Si era civil: El juego continúa
4. Continúa votando hasta que haya un ganador

### 6. Condiciones de Victoria
- **Civiles ganan**: Eliminan a todos los impostores
- **Impostores ganan**: Quedan igual o más impostores que civiles
- **Impostores ganan**: Adivinan la palabra

## 📱 Instalar como PWA

### En Android:

1. Abre la app en Chrome
2. Toca el menú (⋮) > "Añadir a pantalla de inicio"
3. Confirma la instalación
4. Accede desde tu pantalla de inicio

### En iOS:

1. Abre la app en Safari
2. Toca el botón de compartir
3. Selecciona "Añadir a pantalla de inicio"
4. Confirma la instalación

## 🎯 Configuración de Impostores

Puedes elegir el número de impostores manualmente:

- Selecciona de 1 hasta (número de jugadores - 1) impostores
- O activa "Número aleatorio" para sorpresa en cada partida
- Siempre habrá al menos 1 civil

## 🔞 Control Parental - Contenido +18

La aplicación incluye una categoría especial **Adultos (+18)** con contenido explícito:

### Seguridad y Protección
- **Bloqueado por defecto**: La categoría +18 NO es visible ni accesible inicialmente
- **Verificación requerida**: Al intentar activarla, aparece un modal de confirmación de edad
- **Advertencia clara**: Se muestra un aviso sobre el contenido explícito
- **Confirmación explícita**: Requiere confirmar que eres mayor de 18 años

### Cómo Activar
1. Ve a "Configuración" → "Temas"
2. Verás la categoría "Adultos (+18) 🔞" al final de la lista
3. Al hacer clic en el checkbox para activarlo, aparecerá un modal de advertencia
4. Lee el aviso y confirma que eres mayor de 18 años
5. Una vez confirmado, el tema se activará y podrás usarlo en partidas

### Cómo Desactivar
1. Desmarca el checkbox "Adultos (+18) 🔞"
2. La categoría se bloqueará automáticamente
3. Se eliminará de los temas seleccionados
4. La configuración se guarda localmente

**Nota**: Este control parental es una medida de protección básica. La responsabilidad final recae en el usuario y los padres/tutores.

## 🎨 Personalización

### Cambiar Idioma

1. Ve a "Configuración"
2. Selecciona "Español", "English" o "Català"
3. La app se actualiza automáticamente

### Modo Oscuro

1. Ve a "Configuración"
2. Activa "Modo Oscuro"
3. La configuración se guarda automáticamente

## 📂 Estructura del Proyecto

```
impostor-game/
├── index.html              # HTML principal
├── manifest.json           # Configuración PWA
├── service-worker.js       # Service Worker para offline
├── css/
│   └── styles.css          # Estilos completos
└── js/
    ├── app.js              # Navegación e inicialización
    ├── config.js           # Configuración e idiomas
    ├── data.js             # Temas y palabras
    ├── game.js             # Lógica del juego
    └── players.js          # Gestión de jugadores
```

## 🛠️ Tecnologías

- **HTML5**: Estructura semántica
- **CSS3**: Variables CSS, Grid, Flexbox, Animaciones
- **JavaScript Vanilla**: Sin frameworks ni librerías
- **PWA**: Service Worker, Web App Manifest
- **LocalStorage**: Persistencia de configuración

## 🎨 Características de Diseño

- **Paleta moderna**: Colores vibrantes basados en Indigo
- **Transiciones suaves**: Animaciones CSS
- **Botones grandes**: Fáciles de tocar en móvil
- **Feedback visual**: Animaciones al interactuar
- **Responsive**: Adaptable a todos los tamaños

## 🐛 Solución de Problemas

### La app no funciona offline
- Asegúrate de acceder vía servidor HTTP (no file://)
- Verifica que el Service Worker esté registrado (Consola > Application)

### Los iconos no se muestran
- Crea archivos `icon-192.png` e `icon-512.png` en la raíz del proyecto
- O elimina las referencias en `index.html` y `manifest.json`

### Las traducciones no cambian
- Recarga la página después de cambiar el idioma
- Verifica que el navegador soporte localStorage

## 📝 Notas de Desarrollo

### Añadir Nuevos Temas

Edita `js/data.js` y añade tu tema en los tres idiomas (ES, EN, CA):

```javascript
const temasPalabras = {
    es: {
        nuevoTema: [
            // Subtema 1
            'palabra1', 'palabra2', 'palabra3',
            // Subtema 2
            'palabra4', 'palabra5', 'palabra6',
            // ... Mínimo 100 palabras recomendado
        ]
    },
    en: {
        nuevoTema: ['word1', 'word2', 'word3', ...]
    },
    ca: {
        nuevoTema: ['paraula1', 'paraula2', 'paraula3', ...]
    }
};
```

Luego añade la traducción del nombre del tema en `js/config.js`:

```javascript
const traducciones = {
    es: {
        nuevoTema: 'Nuevo Tema'
    },
    en: {
        nuevoTema: 'New Theme'
    },
    ca: {
        nuevoTema: 'Tema Nou'
    }
};
```

**Nota sobre temas adultos**: Si añades contenido explícito, considera añadirlo a la categoría `adultos` existente en lugar de crear una nueva categoría, para mantener el control parental unificado.

### Añadir Nuevos Idiomas

1. Añade el objeto de palabras en `js/data.js`
2. Añade las traducciones en `js/config.js`
3. Añade la opción en el selector de idioma en `index.html`

## 🤝 Contribuciones

Este es un proyecto de código abierto. Siéntete libre de:

- Reportar bugs
- Sugerir nuevas características
- Añadir más palabras a los temas existentes
- Traducir a nuevos idiomas
- Mejorar el diseño

## 📄 Licencia

Este proyecto es de código abierto y está disponible bajo la licencia MIT.

## 🎉 Créditos

Desarrollado con ❤️ usando JavaScript Vanilla.

---

**¡Disfruta encontrando al impostor!** 🕵️‍♂️🕵️‍♀️
