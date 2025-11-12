# 🎨 Studio CreArtes - Website

## 📌 Descripción General

Sitio web profesional para **Studio CreArtes**, estudio de diseño gráfico y soluciones creativas en Panamá. 

El sitio está completamente personalizado con:
- Logo turquesa de Studio CreArtes
- Misión, Visión y Valores de la empresa
- 5 categorías de servicios reales
- Diseño moderno y responsive
- **🌓 Sistema Dark/Light Mode** con negro como protagonista

---

## 🌓 Nuevo: Sistema de Temas

### 🌙 Modo Dark (Predeterminado)
- Fondo negro (#000000) - Color principal del cliente
- Texto blanco brillante
- Cards en gris oscuro elegante
- Perfecto para impresionar con modernidad

### ☀️ Modo Light
- Fondo blanco limpio
- Texto negro nítido
- Cards en blanco puro
- Ideal para legibilidad máxima

**Cambio instantáneo** con botón en header (esquina superior derecha)  
**Preferencia guardada** automáticamente

� **Documentación completa**: Ver `TEMA_DARK_LIGHT.md`

---

## �📂 Estructura del Proyecto

```
creArtes/
├── index.html                      # Archivo HTML principal
├── css/
│   ├── main.css                   # Estilos CSS con sistema dark/light
│   └── main-backup.css            # Backup del diseño anterior
├── js/
│   └── main.js                    # JavaScript + Toggle de tema
├── assets/
│   └── logo-creartes.svg          # Logo SVG de Studio CreArtes
├── TEMA_DARK_LIGHT.md             # 🆕 Documentación del sistema de temas
├── LEEME_DARK_LIGHT.md            # 🆕 Guía simple para el cliente
├── CAMBIOS_IMPLEMENTADOS.md       # Detalle de cambios anteriores
└── README.md                      # Este archivo
```

---

## 🚀 Cómo Usar

### Opción 1: Servidor Local (Recomendado para Desarrollo)

```bash
# Navega a la carpeta del proyecto
cd c:\Users\luisr\Repo-de-desarrollo\creArtes

# Inicia el servidor Python
python -m http.server 8080

# Abre en tu navegador
http://localhost:8080
```

### Opción 2: Abrir Directamente en el Navegador

Haz doble clic en `index.html` (limitado para desarrollo)

---

## 🎯 Secciones del Sitio

### 1. **Header/Navegación**
- Logo de Studio CreArtes (SVG)
- Menú navegable
- Botón móvil responsive
- Enlaces a: Servicios, Nosotros, Portafolio, Contacto

### 2. **Hero (Inicio)**
- Título: "Studio CreArtes: Soluciones Creativas que Hacen Destacar tu Marca"
- Descripción personalizada
- Botones CTA (WhatsApp + Servicios)
- Valores destacados

### 3. **Servicios**
5 Categorías principales:
1. 🎨 Diseño Gráfico Creativo
2. 📣 Publicidad y Marketing Visual
3. 💻 Soluciones Web y Digitales
4. 🎁 Artículos Promocionales
5. 📱 Asesoría y Gestión de Contenidos

### 4. **Nosotros (Misión, Visión, Valores)**
- Misión de la empresa
- Visión a futuro
- 3 Valores clave

### 5. **Portafolio**
- Casos de éxito (pendiente: agregar tus proyectos reales)
- Imágenes de trabajos
- Descripción de resultados

### 6. **FAQ y Beneficios**
- Preguntas frecuentes
- Razones para elegirnos

### 7. **Contacto**
- Formulario de cotización
- Información de contacto
- Integración WhatsApp

### 8. **Footer**
- Logo y tagline
- Información de la empresa
- Enlaces rápidos
- Redes sociales

---

## 🎨 Personalización

### Cambiar Colores de Marca

Edita `css/main.css` líneas 1-40:

```css
:root {
  --primary-color: #0B9B9B;      /* Turquesa */
  --secondary-color: #00D9D9;    /* Turquesa claro */
  --accent-color: #0B9B9B;       /* Acentos */
  /* ... más colores */
}
```

### Actualizar Logo

1. Reemplaza `assets/logo-creartes.svg` con tu logo
2. O edita el SVG actual en cualquier editor (Figma, Adobe XD, etc.)

### Cambiar Información de Contacto

En `index.html`:
- Busca `50712345678` (WhatsApp)
- Reemplaza con tu número real
- Actualiza email en el formulario de contacto

### Agregar Más Servicios

En `index.html` (sección servicios):
```html
<div class="servicio-card">
    <span class="servicio-icon">🎨</span>
    <h3 class="servicio-title">Tu Servicio</h3>
    <!-- ... contenido ... -->
</div>
```

---

## 📝 Contenido a Completar

- [ ] **Fotos del equipo** - Agregar miembros del equipo
- [ ] **Casos de éxito reales** - Proyectos completados
- [ ] **Testimonios** - De clientes satisfechos
- [ ] **Números reales** - Proyectos, años, clientes
- [ ] **Más imágenes** - Para cada servicio
- [ ] **Videos** - Demostraciones de trabajos

---

## 🛠️ Personalización Avanzada

### Modificar Estilos CSS

El archivo `css/main.css` está bien documentado:
- Líneas 1-40: Variables (colores, espaciado, fuentes)
- Líneas 41-100: Estilos globales
- Líneas 101-400: Componentes (botones, cards, etc.)
- Líneas 400+: Secciones específicas

### Agregar JavaScript

En `js/main.js` puedes agregar:
- Animaciones personalizadas
- Lógica de formularios
- Efectos interactivos
- Integración con APIs externas

### Integración de Formulario

El formulario actualmente redirige a WhatsApp. Para integrar con backend:
1. Modifica la función en `js/main.js` (línea ~80)
2. Conecta con un servicio (Firebase, Netlify Forms, backend propio)

---

## 📱 Responsive Design

El sitio es 100% responsive:
- **Desktop**: Layout completo (1280px+)
- **Tablet**: 768px - 1280px
- **Móvil**: <768px

Media queries en CSS: líneas 1000+

---

## 🔍 SEO Optimizado

- ✅ Meta tags descriptivos
- ✅ Estructura HTML semántica
- ✅ Títulos y headings jerarquizados
- ✅ URLs amigables
- ✅ Imágenes con alt text
- ✅ Mobile-first responsive

---

## 📊 Paleta de Colores

| Color | Código | Uso |
|-------|--------|-----|
| Turquesa | #0B9B9B | Principal, botones, acentos |
| Turquesa Oscuro | #077a7a | Hover, sombras |
| Turquesa Claro | #00D9D9 | Secundario, gradientes |
| Blanco | #FFFFFF | Fondo, texto claro |
| Gris Oscuro | #111827 | Fondo footer, textos |

---

## 🚀 Deploy (Publicación)

### Opción 1: Netlify (Recomendado)
1. Sube los archivos a GitHub
2. Conecta con Netlify
3. Auto-deploy en cada push

### Opción 2: GitHub Pages
1. Crea un repositorio
2. Sube los archivos
3. Habilita GitHub Pages en Settings

### Opción 3: Servidor Web Propio
1. FTP/SFTP los archivos
2. Apunta el dominio
3. ¡Listo!

---

## 📞 Contacto & Soporte

Para preguntas sobre:
- **Modificaciones del sitio** - Contacta a tu desarrollador
- **Contenido** - Actualiza directamente en los archivos HTML
- **Estilos** - Edita `css/main.css`
- **Funcionalidad** - Modifica `js/main.js`

---

## 📄 Licencia

Este sitio web es propiedad de **Studio CreArtes** © 2025

---

## ✨ Notas Importantes

1. **Los archivos están optimizados** para producción pero pueden mejorarse
2. **Usa un servidor HTTP local** en desarrollo (no file://)
3. **Respalda tus cambios** regularmente en GitHub o similar
4. **Prueba en múltiples navegadores** antes de publicar
5. **Verifica en móvil** antes de ir a producción

---

**¡Tu sitio web está listo para crecer junto a Studio CreArtes! 🎨✨**
