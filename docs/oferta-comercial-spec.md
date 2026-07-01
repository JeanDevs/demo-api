# Spec: Oferta Comercial — Agents Future AI

> Documento vivo, metodología Spec-Driven Development. Se refina antes de tocar precios/negocio en firme.
> Última actualización: 2026-07-01

## 1. Contexto

Agencia: **Agents Future AI**.
Cliente objetivo: pymes con negocio online (tiendas online y similares), principalmente LatAm (calibrado a Perú).

## 2. Líneas de producto

1. **Agentes** que atienden o venden por el cliente (WhatsApp, chat web).
2. **Landing pages / sitios web.**
3. **Sistemas a medida** (ej: gestión de mesas, cartas digitales).

## 3. Modelo de cobro (decidido)

- Setup fee (pago inicial) + suscripción mensual recurrente.
- Opción de incluir dominio cuando aplique.
- Ventaja competitiva a explotar: **bundle de las 3 líneas bajo una sola suscripción** (el mercado está premiando esto frente a herramientas sueltas).

## 4. Hallazgos de investigación de mercado (validados — no reabrir sin nueva evidencia)

- **Agentes**: estándar de mercado = setup + mensual, **sin cobro por conversación/resolución** (el cobro por uso genera facturas impredecibles, malo para pymes chicas).
  Rango LatAm real: básico USD 20-50/mes, intermedio USD 100-300/mes, avanzado USD 500-1,000/mes.
- **Web/landing**: modelo "Website as a Service" (WaaS) es tendencia 2026 — suscripción en vez de pago único, incluye diseño + hosting + mantenimiento.
  Referencias España (estructura, no copiar el número a Perú): landing simple 150-300€/mes WaaS vs 1.500-3.500€ pago único; tienda a medida 1.200-3.000€/mes WaaS vs 15.000-60.000€ pago único.
- **Sistemas a medida**: se cotizan por proyecto (pago único) + retainer opcional de mantenimiento. Es la línea menos "empaquetable".

## 5. Alcance propuesto por línea (borrador — pendiente de validar con el cliente/negocio)

### 5.1 Agentes (WhatsApp / chat web)

| Dimensión | Básico | Intermedio | Avanzado |
|---|---|---|---|
| Canales | 1 (WhatsApp *o* web chat) | 2 (WhatsApp + web chat) | Multicanal (+ Instagram/Messenger) |
| Función | Responde FAQs + deriva a humano | Responde + toma pedidos/agenda | Responde + vende + upsell + seguimiento post-venta |
| Entrenamiento | Catálogo básico (texto/PDF del cliente) | Catálogo + integración a lista de productos (actualizable) | Catálogo dinámico (sync con inventario/CMS) |
| Límite de conversaciones | Tope mensual (**número sin definir**) | Tope más alto o "uso razonable" (**sin definir**) | Sin tope duro, cláusula de uso justo |
| Handoff a humano | Manual | Con alertas | Con reglas de escalamiento |
| Analytics | Básico (nº conversaciones) | Reporte mensual | Dashboard + insights de ventas |

### 5.2 Web / Landing (WaaS)

- **Landing simple**: 1 página, formulario de contacto, hosting + dominio opcional, X actualizaciones de contenido/mes incluidas (**número sin definir**).
- **Tienda/sitio a medida**: multi-página, catálogo de productos, pasarela de pago, hosting, mantenimiento y actualizaciones incluidas (**cantidad sin definir**).

### 5.3 Sistemas a medida

- Setup = cotización por proyecto (varía según complejidad: gestión de mesas, cartas digitales, etc.).
- Mensual = retainer **opcional** de mantenimiento/soporte (no obligatorio, a diferencia de las otras 2 líneas).
- Decisión abierta: ¿se empuja igual a un retainer mínimo para mantener consistencia con el bundle, o se deja 100% opcional?

### 5.4 Bundle

- Suscripción única combinando las 3 líneas con descuento vs. contratarlas por separado.
- Debe ser la oferta "hero" del messaging (no una línea más).

## 6. Stress-test de posicionamiento (manual — sin plugin de marketing, ver nota abajo)

> Nota: los skills `product-management:product-brainstorming` y `marketing:campaign-plan` no estaban disponibles en la sesión (no instalables desde el teléfono; requieren CLI local). Este stress-test se hizo directamente, sin plugin formal. Si más adelante se instala el plugin, vale la pena re-correr esto y comparar.

**Hipótesis de valor testeada**: "Le vendemos a pymes online de LatAm un paquete todo-en-uno (agente + web + sistema) por suscripción mensual + setup, con precio fijo sin sorpresas, más simple que contratar cada cosa por separado."

### Fortalezas que sostienen la propuesta
- "Sin cobro por uso" en agentes es un diferenciador real: la alternativa típica (WhatsApp Business API con cobro por conversación) genera miedo a la factura sorpresa en una pyme chica.
- El bundle de 3 líneas bajo una suscripción es justo lo que la investigación ya validó como premiado por el mercado frente a herramientas sueltas.
- El modelo WaaS para web está alineado con tendencia 2026, no es una apuesta arriesgada de modelo.

### Riesgos / grietas encontradas (de mayor a menor severidad)

1. **[Alto] Tensión estructural en el bundle.** Sistemas a medida es la única línea que el mercado trata como proyecto + retainer *opcional* (sección 5.3). Si el bundle exige mensualidad fija en las 3 líneas, un prospecto puede sentir que se le fuerza un pago recurrente en algo que naturalmente es puntual, y el bundle se percibe como upsell forzado en vez de beneficio. **Bloqueante antes de nombrar el bundle como oferta hero.**
2. **[Alto] El mensaje "sin cobro por uso" no está en ningún lado como titular de venta hoy** — es una decisión de pricing interna, no un mensaje. Es el argumento más fuerte contra la competencia y debería ser lo primero que escucha un prospecto, no un detalle de la letra chica del contrato.
3. **[Medio] El modelo WaaS es contraintuitivo para una pyme LatAm** acostumbrada a "pago único y ya es mío". Objeción esperada: *"¿por qué pago para siempre por algo que antes compraba una sola vez?"* Si el mensaje no explica el porqué (hosting + mantenimiento + actualizaciones continuas), puede tumbar la conversión de la línea 2 completa.
4. **[Medio] Política de cancelación sin definir es un hueco de confianza, no solo administrativo.** Es de las primeras preguntas que hará un dueño de pyme desconfiado ("si dejo de pagar, ¿pierdo mi web/agente/número?"). Sin respuesta clara no se puede cerrar venta con confianza aunque el precio esté perfecto. Esto sube de prioridad respecto a como estaba listado antes.
5. **[Bajo-Medio] El nombre "Agents Future AI"** enmarca la agencia como especialista en agentes IA, coherente con línea 1 pero puede debilitar credibilidad en líneas 2 y 3 frente a un prospecto que busca "una agencia de webs" y descarta por nombre. No bloqueante, pero a tener en cuenta en el messaging (ej. "más que agentes: tu equipo de tecnología").
6. **[Bajo] Sin casos de éxito todavía (asumido).** Si es así, el mensaje debería apoyarse en garantías/reversibilidad (cancela cuando quieras, soporte reforzado el primer mes) más que en prueba social al inicio.

### Objeciones esperadas de un dueño de pyme (y si la oferta ya las responde)
| Objeción | ¿Resuelta hoy? |
|---|---|
| "¿Qué pasa si cancelo?" | No — pendiente |
| "¿Por qué pago mensual por algo que antes compraba una vez?" | Parcial — falta traducir la lógica WaaS a mensaje |
| "¿Me llega una factura sorpresa si el agente responde mucho?" | Sí, por el modelo de pricing — falta explotarlo como mensaje |
| "¿Puedo empezar con solo el agente y sumar la web después?" | Depende de cómo se defina la puerta de entrada al bundle (abierto) |
| "¿El agente entiende mi catálogo o es un bot genérico?" | Depende del alcance de "entrenamiento con catálogo" (abierto, sección 5.1) |

### Recomendación sobre el bundle como oferta "hero"
Para que funcione como headline necesita, antes de nombrarlo así: (a) una puerta de entrada clara para el cliente que solo quiere 1-2 líneas, no las 3; y (b) resolver la tensión del punto 1 (mensualidad forzada vs. naturaleza de proyecto de "sistemas a medida").

## 7. Pendiente (sin definir — no rellenar con supuestos)

- Precio exacto de setup y mensual por línea/paquete, calibrado a Perú/LatAm (no a precios europeos).
- Números exactos de topes de conversación, actualizaciones/mes incluidas, etc. (alcance fino de cada nivel).
- Alcance exacto de "agente que vende por ti": límites de conversaciones, canales, entrenamiento con catálogo del cliente.
- Nombres comerciales de los paquetes (ej: Basic/Pro/Scale).
- Política de dominio (revender con margen vs costo directo).
- **Política de cancelación** (sube de prioridad tras el stress-test — es objeción de confianza, no solo letra chica).
- Puerta de entrada al bundle: ¿se puede contratar 1-2 líneas sueltas o el bundle es la única forma de entrar?
- Cómo se resuelve la tensión de "sistemas a medida" (proyecto + retainer opcional) dentro de un bundle que promete mensualidad única.

## 8. Siguiente paso

1. Resolver las 4 decisiones bloqueantes que salieron del stress-test (política de cancelación, puerta de entrada al bundle, tensión de sistemas a medida, y explicitar "sin cobro por uso" como mensaje central).
2. Cerrar el alcance fino de cada paquete (números de topes/cantidades marcados como "sin definir" en la sección 5).
3. Cerrar precios exactos por línea/paquete, calibrados a Perú/LatAm.
4. Definir política de dominio.
