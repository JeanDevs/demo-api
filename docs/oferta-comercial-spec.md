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

## 6. Pendiente (sin definir — no rellenar con supuestos)

- Precio exacto de setup y mensual por línea/paquete, calibrado a Perú/LatAm (no a precios europeos).
- Números exactos de topes de conversación, actualizaciones/mes incluidas, etc. (alcance fino de cada nivel).
- Alcance exacto de "agente que vende por ti": límites de conversaciones, canales, entrenamiento con catálogo del cliente.
- Nombres comerciales de los paquetes (ej: Basic/Pro/Scale).
- Política de dominio (revender con margen vs costo directo) y qué pasa si el cliente cancela.
- Stress-test de posicionamiento/mensajería (pendiente pasar por skill de marketing antes de cerrar números).

## 7. Siguiente paso

1. Cerrar el alcance fino de cada paquete (números de topes/cantidades marcados como "sin definir" arriba).
2. Stress-test de posicionamiento y mensajería con skill de marketing.
3. Cerrar precios exactos por línea/paquete, calibrados a Perú/LatAm.
4. Definir política de dominio y cancelación.
