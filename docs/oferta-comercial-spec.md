# Spec: Oferta Comercial — Agents Future AI

> Documento vivo, metodología Spec-Driven Development. Se refina antes de tocar precios/negocio en firme.
> Última actualización: 2026-07-01 (gaps operativos/de negocio agregados como pendientes)

## 1. Contexto

Agencia: **Agents Future AI** *(placeholder — el nombre comercial definitivo aún no está decidido, ver sección 8)*.
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

| Dimensión | Arranque / Starter | Crecimiento / Growth | Escala / Scale |
|---|---|---|---|
| Canales | 1 (WhatsApp *o* web chat) | 2 (WhatsApp + web chat) | Multicanal (+ Instagram/Messenger) |
| Función | Responde FAQs + deriva a humano | Responde + toma pedidos/agenda | Responde + vende + upsell + seguimiento post-venta |
| Entrenamiento | Catálogo básico (texto/PDF del cliente) | Catálogo + integración a lista de productos (actualizable) | Catálogo dinámico (sync con inventario/CMS) |
| Límite de conversaciones | 300/mes | 1,000/mes | Sin tope duro, cláusula de uso justo |
| Handoff a humano | Manual | Con alertas | Con reglas de escalamiento |
| Analytics | Básico (nº conversaciones) | Reporte mensual | Dashboard + insights de ventas |

> El tope de conversaciones es una señal para subir de plan, no una factura extra: si un cliente Arranque/Crecimiento supera el tope, se le invita a upgrade — nunca se le cobra por conversación, para mantener intacto el mensaje "sin cobro por uso" (sección 6.1, decisión 4).
> Nombres de tier (Arranque/Crecimiento/Escala, ES/EN) definidos en sección 5.5. Tabla usa el nombre interno en la columna "Dimensión" y el nombre comercial en el encabezado.

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

### 5.5 Nombres comerciales de los tiers (cerrado 2026-07-01)

Esquema de nombres para los 3 tiers, en español (principal) e inglés (para la landing bilingüe):

| Tier interno | Nombre ES | Nombre EN |
|---|---|---|
| Básico | Arranque | Starter |
| Intermedio | Crecimiento | Growth |
| Avanzado | Escala | Scale |

- Reemplaza "Básico/Intermedio/Avanzado" como etiqueta cara al cliente en Agentes (tabla 5.1) y, cuando aplique, en Web (tabla 5.2).
- El **Bundle** no es un cuarto tier: se nombra como "Suite [Tier]" (ej. "Suite Crecimiento" = tier Crecimiento/Growth de Agente + Web juntos bajo una suscripción).
- Idioma a mostrar depende del idioma de la página (landing bilingüe ES/EN), ambos nombres son oficiales, ninguno es traducción improvisada.

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

## 7. Precios por línea

Moneda: **soles (PEN)**. Tipo de cambio de referencia usado para calibrar contra los rangos LatAm en USD: ~S/ 3.75 por USD (solo referencia interna, el cliente ve precio en soles).

### 7.1 Agentes (cerrado 2026-07-01)

| Paquete | Setup (pago único) | Mensual |
|---|---|---|
| Arranque / Starter | S/ 300 | S/ 89/mes |
| Crecimiento / Growth | S/ 600 | S/ 399/mes |
| Escala / Scale | S/ 1,200 | S/ 1,899/mes |

Calibrado a la punta baja del rango LatAm validado (USD 20-50 / 100-300 / 500-1,000 mensual, sección 4), por poder adquisitivo de Perú. El setup escala según complejidad de integración de cada nivel (catálogo básico → integración a lista de productos → sync con inventario/CMS, columna "Entrenamiento" de la sección 5.1).

### 7.2 Web / Landing (WaaS) — pendiente

Precio sin definir. El criterio de cálculo (cómo traducir la lógica WaaS de "mensual recupera el pago único en X meses" a Perú) queda **pospuesto a propósito**: el usuario decidió no fijarlo ahora y lo retomará más adelante con su propio criterio.

### 7.3 Sistemas a medida

Sin tabla fija — se mantiene cotización por proyecto (sección 5.3), consistente con que el mercado trata esta línea como la menos "empaquetable".

## 8. Pendiente (sin definir — no rellenar con supuestos)

- Precio de setup y mensual de la línea Web (WaaS), incluyendo el criterio de cálculo (sección 7.2).
- Alcance exacto de "agente que vende por ti": canales y entrenamiento con catálogo del cliente ya definidos en la sección 5.1; falta cerrar el detalle operativo de cómo se sincroniza el catálogo dinámico del nivel Avanzado.
- **Nombre comercial definitivo de la agencia**: "Agents Future AI" era solo un placeholder de ejemplo, se va a cambiar (no rellenar con supuestos hasta que el usuario defina el nuevo nombre).
- Política de dominio (revender con margen vs costo directo).
- **Descuento en la cotización de Sistemas a medida para clientes bundle**: decisión pospuesta a propósito — se definirá más adelante, no ahora.
- **% de descuento del bundle Agente+Web** (cuánto más barata es la "Suite" vs. contratar Agente y Web sueltos al mismo tier) — no confundir con el punto anterior (ese es el descuento en Sistemas a medida); este número tampoco está definido todavía.
- **Re-correr el stress-test de posicionamiento (sección 6) con el plugin de marketing real** (`product-management:product-brainstorming` / `marketing:campaign-plan`) cuando el usuario los instale desde su CLI local, y comparar contra el resultado manual.

## 9. Gaps operativos/de negocio detectados (auto-revisión 2026-07-01, sin cubrir aún)

Puntos ciegos encontrados al revisar el spec completo — no son decisiones de producto/pricing como la sección 8, son huecos de ejecución/negocio que pueden invalidar los números ya cerrados si no se resuelven.

1. **[Alto] No hay economía unitaria detrás de los precios cerrados.** Nunca se calculó cuánto cuesta entregar cada tier (API de WhatsApp, hosting, tiempo de soporte/integración de catálogo) contra lo que cobra (sección 7.1). Sin permanencia en Agente/Web, un cliente puede cancelar el mes 1 tras el setup — si S/300 de setup no cubre esa mano de obra, cada cliente que se va rápido es pérdida, no solo cliente perdido.

   **Stack recomendado (borrador, no cerrado):**
   - Modelo de lenguaje para el volumen del día a día: **no usar un modelo Claude/Anthropic como motor de cada mensaje** — el más barato de la familia (Claude Haiku 4.5) lista a USD 1/millón tokens de entrada y USD 5/millón de salida, varias veces más caro por token que alternativas orientadas a volumen (ej. GPT-4o-mini, Gemini Flash, o modelos open-weight vía Groq/Together/Fireworks/DeepInfra). Reservar un modelo premium (de cualquier proveedor) solo para un paso puntual de razonamiento complejo en el tier Escala, no para cada mensaje.
   - RAG (embeddings + vector DB, ej. pgvector/Qdrant) para el catálogo en vez de meter el catálogo completo en cada prompt — evita que el costo escale con el tamaño del catálogo del cliente.
   - Canal WhatsApp vía Meta Cloud API directo (evita markup de un BSP intermediario) si la agencia puede manejar la integración.
   - Límites técnicos duros por cliente (mensajes/hora, turnos máx. antes de escalar a humano) como red de seguridad de margen, independientes del mensaje comercial de "uso justo" que ve el cliente.

   **Casos donde el consumo sube y se pierde margen (de más a menos probable):**
   - Cuota de Meta por conversación de WhatsApp escalando en el tier Escala (sin tope duro) — es un costo pass-through fuera del control de la agencia, más relevante que el costo del modelo de lenguaje en sí.
   - Cliente Arranque/Crecimiento con pico de tráfico (viral, campaña de ads) sin throttling técnico real: sigue recibiendo servicio completo al precio del tier bajo mientras el costo real corre muy por encima de lo presupuestado para ese ciclo.
   - Abuso/prompt injection/loops de reintentos que generan conversaciones de alto volumen y cero valor.
   - Sync de catálogo dinámico (Escala) escalando con el tamaño/frecuencia de actualización del catálogo, no con el número de conversaciones — dos clientes Escala con catálogos muy distintos pagan lo mismo pero cuestan distinto.

   **Caso óptimo:** catálogo chico y estable, tier Arranque con ~100-150 conversaciones reales/mes (bien debajo del tope de 300), conversaciones cortas resueltas sin escalar a humano — costo técnico de unos pocos soles al mes contra S/89 de ingreso.

2. **[Alto] Falta canal de adquisición.** El spec define producto, tiers y precios, pero nada sobre cómo se consiguen los primeros clientes (referidos, comunidades, ads, cold outreach). Sin esto el pricing es teórico — no hay evidencia de campo, solo investigación de escritorio (sección 4).
3. **[Medio] No hay medio de cobro definido.** Precios en soles (sección 7) asumen una forma de cobro recurrente (Yape/Plin, transferencia, tarjeta vía Culqi/Niubiz, etc.) que nunca se especificó. La recurrencia sin permanencia necesita cobro automático o hay que perseguir el pago cada mes manualmente.
4. **[Medio] Falta definir quién entrega el soporte prometido y con qué capacidad.** Compromisos como "2h soporte técnico/mes" (5.2), "reglas de escalamiento" y "dashboard de insights" (5.1, tier Escala) no tienen dueño operativo definido ni límite de cuántos clientes de tier alto se pueden atender antes de que el servicio se degrade.

## 10. Siguiente paso

1. Definir el criterio de cálculo y cerrar precios de la línea Web (WaaS) cuando el usuario lo retome.
2. Definir el nombre comercial definitivo de la agencia y la política de dominio.
3. Definir el % de descuento bundle→Sistemas a medida cuando se retome ese punto.
4. Resolver los gaps operativos de la sección 9 (economía unitaria, canal de adquisición, medio de cobro, capacidad de soporte) — priorizados como bloqueantes reales antes de vender en firme.
