# 🌐 Simulador de Exámenes de Direccionamiento IPv4

Aplicación web **estática de un solo archivo** para practicar y autoevaluar conocimientos de direccionamiento IPv4. Ideal para estudiantes de redes de computadoras que se preparan para un examen tipo cuestionario.

Incluye **4 módulos de práctica por tema** y un **simulacro de examen completo** con 10 preguntas aleatorias calificadas sobre **20 puntos** (nota vigesimal).

---

## ✨ Características principales

- **4 módulos de práctica independientes:**
  1. **Clases de IP** → clase (A/B/C), máscara por defecto y porciones de red/host.
  2. **Prefijos y Máscaras** → conversión bidireccional `/X` ↔ notación decimal.
  3. **Cálculo de Hosts** → de máscara a hosts (`2^N - 2`) y diseño de máscara según cantidad de PCs.
  4. **Red Base y Broadcast** → red base, primer/último IP válido, broadcast y siguiente red.
- **Simulacro de examen:** 10 preguntas aleatorias mezclando los 4 temas, calificadas sobre 20 puntos (aprueba con 13).
- **Ejercicios infinitos:** cada clic genera un ejercicio nuevo con valores aleatorios.
- **Retroalimentación inmediata:** casillas en verde/rojo con pistas específicas para cada campo incorrecto.
- **Ver solución completa:** muestra la respuesta y la explicación paso a paso sin perder tus respuestas (puedes volver a ellas).
- **"Coquito": tabla de consulta** con conversión de bits por octeto, saltos de red, clases y fórmulas clave.
- **Interfaz oscura y responsive** (se adapta a móvil, tablet y escritorio).
- **Puntaje parcial por pregunta:** cada campo acertado suma dentro de la nota final.

## 🛠️ Tecnologías utilizadas

| Tecnología | Uso |
|---|---|
| **HTML5** | Estructura semántica de la interfaz |
| **CSS3** | Diseño, tema oscuro, animaciones y layout responsive (Grid/Flexbox) con variables CSS |
| **JavaScript (Vanilla JS)** | Toda la lógica: generación aleatoria de ejercicios, validación y calificación |

> 📦 **Cero dependencias.** No usa frameworks, librerías, npm ni Node.js. Todo está en un único archivo.

## 🚀 Uso e instalación

No hay nada que instalar. El proyecto es 100% estático:

### Opción 1 — Abrir directamente (la más rápida)

1. Descarga o clona el repositorio.
2. Haz doble clic en **`practica_redes.html`**.
3. Se abrirá en tu navegador predeterminado (Chrome, Firefox, Edge...). ¡Listo!

### Opción 2 — Con Live Server (recomendado para desarrollo)

1. Abre la carpeta en **Visual Studio Code**.
2. Instala la extensión **Live Server**.
3. Haz clic derecho sobre `practica_redes.html` → **"Open with Live Server"**.
4. El navegador se abrirá con recarga automática al guardar cambios.

### Opción 3 — Servidor local (opcional)

```bash
# Con Python 3
python -m http.server 8000
# Luego visita http://localhost:8000
```

## 📁 Estructura del proyecto

```
practicas_redes/
├── practica_redes.html   # Aplicación completa (HTML + CSS + JS en un solo archivo)
├── .gitignore            # Archivos ignorados por Git
└── README.md             # Documentación del proyecto
```

## 📖 Cómo usar la aplicación

1. **Elige un tema** en la barra de pestañas (1 al 4) o entra al **Simulacro Examen**.
2. **Responde** los campos del ejercicio y pulsa **"Comprobar Respuesta"**.
3. Si algo sale mal, lee las **pistas rojas** y corrige; si quieres la respuesta, usa **"Ver Solución Completa"**.
4. Pulsa **"Refrescar / Otro Ejercicio"** para generar uno nuevo.
5. En el modo examen, responde las 10 preguntas y pulsa **"Calificar Examen"** para ver tu nota sobre 20.

---

> 💡 *Proyecto académico de prácticas de redes — Semana 9/10. Sin dependencias, sin build, sin excusas: solo abre el archivo y practica.*