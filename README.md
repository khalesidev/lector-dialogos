# Teleprompter Web - Enfoque Directo a Cámara 🎥

Aplicación web de **teleprompter profesional** diseñada específicamente para grabadores de video, creadores de contenido, docentes y oradores que necesitan leer un guion frente a su computadora manteniendo un contacto visual natural con la lente, **sin que se note que están leyendo**.

---

## 🌟 Características Principales

### 1. Lectura Anti-Movimiento Ocular (Anti-Saccadic)
* **Texto centrado y pegado arriba:** El texto corre inmediatamente debajo de la cámara de la PC o laptop, minimizando el ángulo entre el texto y la lente.
* **Columna estrecha ajustable (por defecto 480 px):** Al mantener pocas palabras por línea, la visión periférica capta las frases completas, eliminando el movimiento horizontal de los ojos de izquierda a derecha.

### 2. Control de Velocidad Humana Calibrada (0.5x a 6.0x)
* **Ajuste fino decimal (pasos de 0.1):** Sin saltos bruscos. Variaciones suaves de apenas 2.5% por nivel.
* **Velocidades lentas incorporadas (0.5x y 0.8x):** Pensadas para ensayos pausados o locución solemne.
* **Rango conversacional ideal (2.0x a 3.0x):** Calibrado al ritmo estándar de habla en español (130-150 palabras por minuto).

### 3. Anclaje Inteligente de Tamaño de Fuente
* Modificar el tamaño de letra **no desplaza el texto**: el sistema detecta qué oración tienes frente a la guía de lectura y recalcula el scroll en tiempo real para mantener la frase que estás leyendo totalmente inmóvil.
* Si te encuentras al inicio, el texto permanece firme en el margen superior.

### 4. Modo Pantalla Completa Instantáneo (<kbd>F</kbd> / <kbd>F11</kbd>)
* Oculta las barras de pestañas y de direcciones del navegador, llevando la primera línea a escasos milímetros del lente físico de la cámara web.

### 5. Luz de Estado Tally (Indicador de Cámara)
* Cápsula superior con indicador visual de estado:
  * 🔴 **Grabando / Rodando:** Titila suavemente para recordar mantener la mirada fija en el lente.
  * 🔵 **Pausado / En espera:** Indica que el sistema está listo.

### 6. Controles Estrictamente Inferiores
* Todo el panel de control se encuentra anclado en el borde inferior con diseño de cristal esmerilado (*glassmorphism*), sin interferir nunca con la zona de lectura superior.
* Iconografía vectorial nítida basada en **Lucide Icons**.

---

## ⌨️ Atajos de Teclado

| Tecla | Acción |
| :--- | :--- |
| <kbd>Espacio</kbd> | Iniciar o pausar el desplazamiento |
| <kbd>▲</kbd> | Aumentar velocidad (+0.1x) |
| <kbd>▼</kbd> | Disminuir velocidad (-0.1x) |
| <kbd>R</kbd> | Reiniciar el texto al inicio |
| <kbd>F</kbd> | Alternar Pantalla Completa |
| <kbd>Esc</kbd> | Abrir / Cerrar el editor de guion |

---

## 🚀 Cómo Usar

No requiere servidores, dependencias ni instalación de Node.js.

1. Abre el archivo [`index.html`](index.html) con tu navegador habitual (Google Chrome, Microsoft Edge, Mozilla Firefox o Brave).
2. Haz clic en **"Editar Guion"** (o presiona <kbd>Esc</kbd>) y pega el texto de tu guion.
3. Presiona **"Pantalla Completa"** (<kbd>F</kbd>) para pegar el texto a la cámara física.
4. Ajusta el tamaño de letra y la velocidad a tu gusto.
5. Presiona la **Barra Espaciadora** (<kbd>Espacio</kbd>): se activará la cuenta regresiva de 3 segundos para que fijes tu mirada en la cámara y comiences a grabar.

---

## 💡 Consejos para que no se note que lees

1. **Distancia a la pantalla:** Siéntate a unos 60-80 cm de tu monitor o laptop. A esa distancia, el ángulo visual entre el borde superior del texto y la cámara se reduce a casi 0°.
2. **Columna angosta:** Mantén el ancho del texto entre 420 px y 500 px. Cuanto más estrecha la columna, menor será el movimiento de tus pupilas.
3. **Parpadeo y gesticulación natural:** No te quedes inmóvil con los ojos fijos. Parpadea con naturalidad, asiente ocasionalmente o acompaña tus palabras con ademanes de manos.
4. **Ajuste de velocidad sobre la marcha:** Durante la toma, puedes acelerar o desacelerar con las flechas <kbd>▲</kbd> / <kbd>▼</kbd> sin necesidad de mirar el teclado ni tocar el mouse.

---

## 🛠️ Tecnologías Utilizadas

* **HTML5 Semántico**
* **CSS3 Moderno:** Flexbox, variables CSS, backdrop-filter (*glassmorphism*), gradientes radiales optimizados para pantallas oscuras/OLED.
* **JavaScript Puro (Vanilla JS):** Animación fluida con `requestAnimationFrame`, anclaje geométrico con `getBoundingClientRect` y soporte de Fullscreen API.
* **Iconos:** SVGs vectoriales integrados inspirados en el ecosistema **Lucide**.
