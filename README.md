# Code & Popcorn - Documentación Técnica

## Desglose del Desarrollo

### 1. Arquitectura HTML5 (Estructura)
El sitio está construido bajo estándares de *HTML Semántico*, lo que garantiza accesibilidad y un mejor indexado en buscadores:
- *Header dinámico*: No es solo una imagen; es un contenedor con una capa de fondo (background-image) que permite superponer texto real. Esto es vital para el SEO, 
ya que los buscadores pueden leer "Code & Popcorn" como texto y no como una simple imagen.
- *Sección de Contenidos (<main>)*: Organizada mediante artículos (<article>). Cada película es una entidad independiente, lo que facilita futuras expansiones 
(como añadir comentarios o valoraciones).

### 2. Capa de Estilos (CSS3 Avanzado)
El reto principal fue la *legibilidad sobre imágenes complejas*:
- *Técnica de Overlay*: Se implementó background-image: linear-gradient(rgba(0,0,0,0.6), ...), url(...). Esta doble capa permite oscurecer el collage de pósteres un 
60%, haciendo que el texto blanco y amarillo resalte sin perder la estética cinematográfica de fondo.
- *Sistema de Centrado (Flexbox)*: Se utilizó display: flex con justify-content: center y align-items: center en el hero. Esto garantiza que el título esté 
perfectamente alineado sin importar si el usuario entra desde un móvil o un monitor 4K.
- *Tratamiento de Imágenes de Cartelería*: Para evitar que los pósteres de diferentes proporciones rompan el diseño, se aplicó object-fit: cover. Esto recorta la 
imagen proporcionalmente para llenar el contenedor asignado sin deformar las caras de los actores.

### 3. Estética "Dark Mode"
Se eligió una paleta de colores #1a1a1a (Gris Eerie) para el fondo y #f1c40f (Amarillo Flat) para acentos. Esta combinación reduce la fatiga visual y emula la 
interfaz de plataformas como Netflix o Disney+.

### 4. Recursos Multimedia
- *Collage Personalizado*: Imagen horizontal que recopila hitos del cine desde 2004 (Era Post-Matrix), cubriendo géneros desde el terror psicológico 
hasta la animación modern
