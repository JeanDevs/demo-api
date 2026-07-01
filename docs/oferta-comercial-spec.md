# Spec: Oferta Comercial — Agents Future AI

> Documento vivo, metodología Spec-Driven Development. Se refina antes de tocar precios/negocio en firme.
> Última actualización: 2026-07-01 (alcance de paquetes cerrado)

## 1. Contexto

Agencia: **Agents Future AI**.
Cliente objetivo: pymes con negocio online (tiendas online y similares), principalmente LatAm (calibrado a Perú).

## 2. Líneas de producto

1. **Agentes** que atienden o venden por el cliente (WhatsApp, chat web).
2. **Landing pages / sitios web.**
3. **Sistemas a medida** (ej: gestión de mesas, cartas digitales).

## 3. Modelo de cobro (decidido)

- Setup fee (pago inicial) + suscripción mensual recurrente para **Agentes** y **Web**.
- **Sistemas a medida** queda fuera de la mensualidad única (ver sección 6.1, decisión 3): siempre proyecto (pago único) + retainer opcional, cotizado aparte.
- Opción de incluir dominio cuando aplique.
- Ventaja competitiva a explotar: **bundle de Agente + Web bajo una sola suscripción**, con descuento en la cotización de Sistemas a medida como upsell de proyecto para clientes bundle (el mercado premia esto frente a herramientas sueltas).
- Cualquier línea puede contratarse suelta a precio individual; el bundle es el incentivo de mejor precio, no la única puerta de entrada (ver sección 6.1, decisión 2).
- Permanencia: sin permanencia en Agente y Web (cancela cuando quieras); permanencia mínima en el retainer de Sistemas a medida (ver sección 6.1, decisión 1 — duración exacta aún pendiente, sección 7).

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
| Límite de conversaciones | 300/mes | 1,000/mes | Sin tope duro, cláusula de uso justo |
| Handoff a humano | Manual | Con alertas | Con reglas de escalamiento |
| Analytics | Básico (nº conversaciones) | Reporte mensual | Dashboard + insights de ventas |

> El tope de conversaciones es una señal para subir de plan, no una factura extra: si un cliente Básico/Intermedio supera el tope, se le invita a upgrade — nunca se le cobra por conversación, para mantener intacto el mensaje "sin cobro por uso" (sección 6.1, decisión 4).

### 5.2 Web / Landing (WaaS)

- **Landing simple**: 1 página, formulario de contacto, hosting + dominio opcional, 2 actualizaciones de contenido menores/mes incluidas (texto/imágenes; cambios grandes de diseño se cotizan aparte).
- **Tienda/sitio a medida**: multi-página, catálogo de productos, pasarela de pago, hosting, actualizaciones rutinarias ilimitadas (productos/precios) + 2 horas de soporte técnico/mes incluidas.

### 5.3 Sistemas a medida

- Setup = cotización por proyecto (varía según complejidad: gestión de mesas, cartas digitales, etc.).
- Mensual = retainer **opcional** de mantenimiento/soporte (no obligatorio, a diferencia de las otras 2 líneas).
- Decisión abierta: ¿se empuja igual a un retainer mínimo para mantener consistencia con el bundle, o se deja 100% opcional?

### 5.4 Bundle

- Suscripción única de **Agente + Web** con mejor precio que contratar cada una suelta.
- **Sistemas a medida no forma parte de la mensualidad del bundle** (decisión cerrada en 6.1): se cotiza como proyecto aparte, con descuento en esa cotización para clientes que ya tienen el bundle.
- Cualquier línea (incluido Agente o Web solos) puede contratarse suelta a precio individual — el bundle no es obligatorio para acceder a la agencia, es el incentivo de mejor precio.
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

## 6.1 Decisiones cerradas tras el stress-test (2026-07-01)

1. **Política de cancelación/permanencia**: sin permanencia en Agente y Web (cancela cuando quieras); permanencia mínima de **3 meses** en el retainer de Sistemas a medida, para recuperar la inversión de desarrollo custom.
2. **Puerta de entrada al bundle**: cualquier línea se puede contratar suelta a precio individual. El bundle no es la única forma de entrar, es el incentivo de mejor precio si el cliente toma Agente + Web juntos.
3. **Tensión de Sistemas a medida**: queda fuera de la mensualidad única del bundle. Sigue siendo proyecto (pago único) + retainer opcional, cotizado aparte, con descuento en esa cotización para clientes que ya tienen el bundle Agente + Web. Esto **redefine el bundle**: ya no es "3 líneas bajo una suscripción" sino "Agente + Web bajo una suscripción, con beneficio de precio en Sistemas a medida como upsell de proyecto" (aplicado en secciones 3 y 5.4).
4. **Mensaje "sin cobro por uso"**: se eleva de decisión de pricing a principio de messaging explícito. Debe aparecer en el primer contacto de venta, en la página de precios y en el contrato — no solo vivir en la letra chica.
   - Tagline de trabajo: *"Un precio fijo cada mes. Sin sorpresas en tu factura, sin importar cuánto vendas."*

## 7. Pendiente (sin definir — no rellenar con supuestos)

- Precio exacto de setup y mensual por línea/paquete, calibrado a Perú/LatAm (no a precios europeos).
- Alcance exacto de "agente que vende por ti": canales y entrenamiento con catálogo del cliente ya definidos en la sección 5.1; falta cerrar el detalle operativo de cómo se sincroniza el catálogo dinámico del nivel Avanzado.
- Nombres comerciales de los paquetes (ej: Basic/Pro/Scale).
- Política de dominio (revender con margen vs costo directo).
- **Descuento en la cotización de Sistemas a medida para clientes bundle**: decisión pospuesta a propósito — se definirá más adelante, no ahora.

## 8. Siguiente paso

1. Cerrar precios exactos por línea/paquete, calibrados a Perú/LatAm (con el alcance de la sección 5 ya cerrado).
2. Definir nombres comerciales de los paquetes y política de dominio.
3. Definir el % de descuento bundle→Sistemas a medida cuando se retome ese punto.
