# DESIGN.md — Synesis AI

> Sistema de marca de **Synesis AI** (@synesis_ai), extraído del feed de Instagram.
> Úsalo como referencia para cualquier pieza: posts, carruseles, reels, web, propuestas o prompts de generación de imagen.

---

## 1. Esencia de marca

| | |
|---|---|
| **Qué es** | IA (agentes conversacionales) para **residencias de mayores**. |
| **Problema que ataca** | Consultas de familias que se responden tarde, se enfrían y acaban en plazas perdidas. |
| **Promesa** | *Ayudamos a residencias a no perder ni una plaza.* |
| **Posicionamiento** | Nicho absoluto. "No hago IA para todo el mundo." Especialista, no agencia generalista. |
| **Diferencial** | Un agente que entiende urgencias reales, adaptado al proceso real de admisión de cada centro (no un chatbot genérico). |
| **Tensión emocional central** | **Tiempo / urgencia** (relojes, cuentas atrás, hielo, teléfonos cortados) frente a **calidez / hogar** (lámparas, sillones, mantas, luz cálida). |

**Pilares de contenido**

1. **Dolor invisible** — plazas que se pierden sin que nadie lo note.
2. **Urgencia** — minutos y segundos que deciden si la familia elige tu residencia o la de al lado.
3. **Método** — cómo trabajo: escucho, adapto, construyo.
4. **Diferenciación** — chatbot ≠ agente; genérico ≠ hecho a medida.
5. **Lo humano** — detrás de cada consulta hay una familia y una persona mayor.

---

## 2. Paleta de color

Valores muestreados directamente de las publicaciones (pueden variar ±5% por compresión de Instagram).

### Primarios

| Token | HEX | Uso |
|---|---|---|
| `--navy-deep` | `#12134E` | Fondo principal oscuro (posts de urgencia, "Ahora mismo…", "1:59"). |
| `--navy-ink` | `#0D133B` | Fondo nocturno / tecnológico ("¿URGENTE?"). |
| `--navy-text` | `#1A1B4B` | Texto titular sobre fondos claros (serif "Ni una plaza", "errores"). |
| `--cream` | `#FDFCF3` | Fondo claro principal, papel cálido. |
| `--cream-warm` | `#F4F2E9` | Fondo claro alternativo, ligeramente más cálido. |

### Acentos (marca / IA)

| Token | HEX | Uso |
|---|---|---|
| `--synesis-blue` | `#5267F5` | Azul del logo, inicio de degradados, elementos "IA". |
| `--electric-blue` | `#4B55F2` | Brillos y objetos iluminados (llave, cable). |
| `--sky-blue` | `#5884DA` | Texto en degradado (parte superior). |
| `--cyan-glow` | `#97FCFD` | Dígitos de reloj, glow, HUD tecnológico. |
| `--mint` | `#94FFD1` | Final del degradado, palabra destacada ("gente"), check. |
| `--mint-soft` | `#77CDB9` | Iconos de check, versión suave del mint. |
| `--ring-cyan` | `#7BC6FB` | Anillos/trazos de luz sobre fondos claros. |

### Contraste / alerta

| Token | HEX | Uso |
|---|---|---|
| `--coral` | `#DD674D` | Subrayados a mano, línea vertical de énfasis, tachados, chispas de "corte". Úsalo con moderación (≤5% de la pieza). |

### Neutros cálidos (fotografía / ambiente)

| Token | HEX | Uso |
|---|---|---|
| `--linen` | `#E7DCCB` | Fondos fotográficos beige, paredes. |
| `--wood` | `#5E4830` | Madera, mobiliario, interiores de residencia. |
| `--espresso` | `#251608` | Sombras cálidas. |
| `--charcoal` | `#131A29` | Fondo oscuro fotográfico (manos, bastón). |
| `--slate` | `#646C7E` | Texto secundario sobre oscuro. |

### Degradado firma

```css
--gradient-synesis: linear-gradient(90deg, #5267F5 0%, #5884DA 35%, #7BC6FB 65%, #94FFD1 100%);
```
Se usa en: logo (símbolo ∞), palabras clave en titulares ("residencias de mayores", "gente"), trazos de luz, llave iluminada.

### Proporción recomendada
- **60%** navy o cream (nunca ambos al 50% en la misma pieza: elige modo oscuro o modo claro).
- **30%** fotografía cálida / neutros.
- **10%** acentos (degradado azul→mint). El coral, solo como subrayado o señal.

---

## 3. Tipografía

Las fuentes se han identificado visualmente; son las equivalentes más cercanas disponibles en Google Fonts.

| Rol | Fuente sugerida | Estilo | Dónde aparece |
|---|---|---|---|
| **Display serif** (titular emocional) | **Playfair Display** / DM Serif Display | Bold, condensado, interlineado muy apretado (0.9–1.0) | "3 errores que hacen perder plazas", "Ayudamos a residencias", "Un chatbot no es lo mismo…" |
| **Serif itálica** (énfasis) | **Playfair Display Italic** | Bold Italic | "*te han enfriado*", "*sin que nadie se dé cuenta*", "*hablo con cada centro*" |
| **Condensada de impacto** | **Bebas Neue** / Oswald Bold / Barlow Condensed | Mayúsculas o mixta, muy alta | "¿URGENTE?", "Hago IA para residencias de mayores", "NI UNA PLAZA" |
| **Serif espaciada elegante** | **Cormorant Garamond** | Mayúsculas, tracking +200 a +300 | "LA PLAZA NO ESPERA." |
| **Sans geométrica** (cuerpo y anuncios) | **Montserrat** / Poppins | Bold para titular, Regular para cuerpo | "Ahora mismo, una familia está escribiendo…" |
| **Cuerpo / subtítulos** | **Inter** | Regular 400–500 | Subtítulos pequeños, handle @synesis_ai |
| **Dígitos** | Flip clock / 7 segmentos (DSEG7) | — | "1:59", "00:30" |

**Reglas**
- Máximo **2 familias** por pieza (display + cuerpo).
- Mezcla firma: **serif bold recta + serif italic** en la misma frase para marcar la palabra que duele.
- Titulares grandes que ocupan 40–60% del lienzo; el texto puede sangrar fuera del borde (recurso del feed para crear continuidad en la cuadrícula).
- Subtítulo siempre mucho más pequeño (≈ 25–30% del tamaño del titular).

---

## 4. Tono de voz

**Personalidad:** especialista cercano, directo, sereno. Habla como alguien que conoce las residencias por dentro, no como una startup de tecnología.

| Es | No es |
|---|---|
| Directo y concreto | Técnico o lleno de jerga |
| Empático con familias y equipos | Alarmista o culpabilizador |
| Urgente con calma | Agresivo / "vendehumo" |
| Especialista de nicho | Generalista "IA para todo" |
| Primera persona, artesanal ("hablo", "adapto") | Corporativo impersonal |

**Recursos de escritura**
- **Pregunta incómoda** como gancho: *"¿Cuántas consultas se te han enfriado este mes sin que lo supieras?"*
- **Escena en presente**: *"Ahora mismo, una familia está escribiendo a una residencia."*
- **Contraste negación/afirmación**: *"No hago IA para todo el mundo. Hago IA para residencias de mayores."*
- **Números y tiempos concretos**: 30 segundos, 10 minutos, 3 errores.
- **Lo invisible**: *"sin que nadie se dé cuenta"*, *"probablemente no lo sepas todavía"*.
- **Frases cortas de cierre** tipo eslogan: *"La plaza no espera. Cada consulta cuenta."*

**Vocabulario propio**
plaza · consulta · familia · residencia · centro · admisión · urgencia · enfriar · perder · responder · minutos · proceso real · agente

> ⚠️ **Coherencia de persona:** el feed alterna *"Hago / Adapto / Hablo"* (yo) con *"Ayudamos"* (nosotros). Recomendación: **primera persona singular** como voz principal (refuerza lo artesanal y cercano) y reservar "nosotros" solo para el claim de marca.

---

## 5. Frases que uso (banco de copy)

**Claims**
- Ayudamos a residencias a no perder **ni una plaza**.
- La plaza no espera. Cada consulta cuenta.
- No hago IA para todo el mundo. Hago IA para residencias de mayores.

**Ganchos**
- ¿Cuántas consultas se te han enfriado este mes sin que lo supieras?
- Ahora mismo, una familia está escribiendo a una residencia.
- Si nadie responde en 10 minutos, está hablando con la de al lado.
- 3 errores que hacen perder plazas sin que nadie se dé cuenta.
- Señales de que estás perdiendo plazas sin darte cuenta. Probablemente no lo sepas todavía.
- ¿Urgente? Cómo saber si una consulta es urgente en los primeros 30 segundos.

**Diferenciación y método**
- Un chatbot no es lo mismo que un agente que entiende una urgencia real.
- Adapto el agente a tu proceso real de admisión.
- Antes de construir nada, hablo con cada centro sobre cómo gestiona hoy sus consultas.

---

## 6. Frases que nunca uso

*(Derivadas del posicionamiento y tono del feed; ajústalas a tu criterio.)*

- ❌ "Revoluciona tu negocio con IA" / "El futuro es ahora" — genérico y vacío.
- ❌ "IA para cualquier empresa / sector" — contradice el nicho.
- ❌ "Sustituye a tu personal" / "Ahorra en plantilla" — la IA apoya al equipo, no lo reemplaza; tema muy sensible en cuidados.
- ❌ "Chatbot" para describir mi producto — siempre **agente**.
- ❌ "Leads", "funnel", "convertir clientes", "cerrar ventas" — se habla de **familias, consultas y plazas**.
- ❌ "Abuelos", "viejitos", "ancianos" — siempre **personas mayores / residentes**.
- ❌ "Solución innovadora de última generación", "disruptivo", "game changer".
- ❌ Anglicismos innecesarios (automation, AI-powered, workflow).
- ❌ Urgencia falsa de venta: "¡Solo hoy!", "Plazas limitadas", "¡No te lo pierdas!".
- ❌ Emojis en exceso o signos de exclamación múltiples.
- ❌ Culpabilizar: "Lo estás haciendo mal" → mejor "probablemente no lo sepas todavía".

---

## 7. Estilo visual

### Dos modos que se alternan en la cuadrícula

**A. Modo Urgencia (oscuro / tecnológico)**
- Fondo navy profundo `#12134E`–`#0D133B` con partículas, bokeh o línea de pulso.
- Objetos-símbolo con **glow cian/mint**: reloj flip "1:59", dígitos "00:30", móvil, llave luminosa.
- Tipografía blanca condensada, gran tamaño.

**B. Modo Hogar (claro / editorial cálido)**
- Fondo crema `#FDFCF3` o fotografía con luz cálida de tarde.
- Escenas de residencia **sin personas o con manos**: sillón con manta, lámpara encendida, mostrador de recepción con libreta y teléfono, bastón.
- Serif navy grande con itálicas de énfasis.

### Metáfora visual (firma de la marca)
Un objeto cotidiano que representa la consulta perdida o el tiempo:
- 🧊 Móvil congelado en un bloque de hielo → "consultas enfriadas".
- ☎️ Cable de teléfono cortado → "errores que hacen perder plazas".
- 🔑 Llaves genéricas vs. llave luminosa con ∞ → "agente a tu medida".
- 💡 Lámpara envuelta en manta → calidez / cuidado.
- ⏱️ Reloj flip y cuenta atrás → urgencia.
- Línea de luz azul-mint que atraviesa la escena (rastro de la IA).

### Fotografía
- Fotorrealista, aspecto editorial/3D de alta calidad.
- Luz cálida lateral (golden hour), sombras suaves, profundidad de campo corta.
- Paleta de madera, lino, beige; nunca fluorescente ni hospitalaria.
- Personas: preferir **manos y detalles**; si aparece una persona, expresión de preocupación contenida (familiar con el móvil).

### Recursos gráficos
- Degradado azul→mint en palabras clave y trazos de luz.
- Subrayado a mano en coral bajo una palabra ("UNA").
- Línea vertical coral como marcador junto al titular.
- Texto tachado en coral para lo que **no** eres.
- Collage de papel rasgado + bocetos a lápiz (posts de método).
- Notificación/burbuja de chat flotante con icono de reloj.

### Composición
- Formato **4:5 vertical** (1080×1350) o 1:1.
- Titular arriba-izquierda, imagen-símbolo en el centro/derecha.
- Margen generoso; mucho aire alrededor del objeto.
- El texto puede cortarse en el borde para enlazar visualmente con el post vecino (efecto cuadrícula continua).
- Logo **Synesis AI** (símbolo ∞ en degradado + wordmark) abajo a la derecha o centrado arriba en anuncios; handle `@synesis_ai` pequeño abajo.

### Prompt base para generación de imagen
```
Fotografía editorial fotorrealista, [OBJETO METAFÓRICO] en [interior cálido de residencia
de mayores / fondo navy profundo #12134E], luz cálida lateral de tarde, sombras suaves,
profundidad de campo corta, paleta beige, madera y lino con un rastro de luz azul-cian
(#5267F5 → #94FFD1), minimalista, mucho espacio negativo arriba a la izquierda para texto,
formato 4:5, sin texto, sin logotipos.
```

---

## 8. Checklist antes de publicar

- [ ] ¿Habla de **plazas, consultas, familias o residencias**?
- [ ] ¿El gancho cabe en una línea y genera una pregunta o una escena?
- [ ] ¿Modo claro **o** oscuro (no mezclado)?
- [ ] ¿Máximo 2 tipografías y 1 acento de color dominante?
- [ ] ¿Hay una metáfora visual en vez de un "robot" o un cerebro digital?
- [ ] ¿Logo o @synesis_ai presentes y discretos?
- [ ] ¿Cero frases de la lista "nunca uso"?
