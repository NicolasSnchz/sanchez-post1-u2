# Checklist heurístico

## Hallazgos documentados

### H1-A
- **Heurística:** H8 - Estética y diseño minimalista
- **Pantalla / contexto:** Resultados de búsqueda
- **Descripción:** La pantalla de resultados presenta una alta densidad de información por producto, incluyendo promociones, descuentos, cuotas, envíos y etiquetas visuales adicionales. Esta acumulación de elementos compite por la atención del usuario y dificulta la comparación rápida entre opciones.
- **Evidencia:** A1_resultados_busqueda.jpg
- **Severidad tentativa:** 2

### H2-A
- **Heurística:** H1 - Visibilidad del estado del sistema
- **Pantalla / contexto:** Resultados tras aplicar filtro
- **Descripción:** Después de aplicar filtros, el sistema no siempre comunica de forma suficientemente explícita qué criterio quedó activo ni cómo cambió el conjunto de resultados. Esto puede generar incertidumbre sobre si el filtro se aplicó correctamente o si el listado mostrado corresponde realmente a la selección hecha por el usuario.
- **Evidencia:** A2_resultados_filtrados.jpg
- **Severidad tentativa:** 2

### H3-A
- **Heurística:** H4 - Consistencia y estándares
- **Pantalla / contexto:** Exploración de resultados refinados
- **Descripción:** La organización de controles y etiquetas comerciales en la pantalla de exploración puede dificultar la identificación inmediata de las acciones principales, ya que elementos promocionales y opciones de refinamiento comparten protagonismo visual con la información esencial de los productos. Esto afecta la claridad del flujo de búsqueda.
- **Evidencia:** A3_resultados_ordenados.jpg
- **Severidad tentativa:** 2

## Hallazgos - Flujo B

### H4-B
- **Heurística:** H8 - Estética y diseño minimalista
- **Pantalla / contexto:** Encabezado del detalle del producto
- **Descripción:** La parte superior del detalle del producto concentra demasiados elementos compitiendo visualmente entre sí, como imagen, precio, descuentos, cuotas, promociones y etiquetas comerciales. Esta sobrecarga dificulta identificar con rapidez la información más importante para decidir si el producto es relevante.
- **Evidencia:** B1_detalle_producto_superior.jpg
- **Severidad tentativa:** 2

### H5-B
- **Heurística:** H6 - Reconocimiento antes que recuerdo
- **Pantalla / contexto:** Sección de envío, vendedor y condiciones
- **Descripción:** La información clave para decidir la compra se encuentra distribuida en distintos bloques separados dentro del detalle. El usuario debe recordar datos vistos anteriormente, como precio, condiciones de envío y confianza del vendedor, para integrarlos mentalmente y tomar una decisión, en lugar de encontrarlos agrupados de forma más directa.
- **Evidencia:** B2_envio_vendedor_condiciones.jpg
- **Severidad tentativa:** 2

### H6-B
- **Heurística:** H1 - Visibilidad del estado del sistema
- **Pantalla / contexto:** Descripción, opiniones o información técnica del producto
- **Descripción:** El detalle del producto no siempre comunica con suficiente claridad qué información es prioritaria dentro del recorrido de evaluación, ya que varias secciones relevantes quedan dispersas a lo largo de un desplazamiento extenso. Esto puede hacer que el usuario no tenga certeza inmediata sobre dónde encontrar la información más útil para validar su decisión de compra.
- **Evidencia:** B3_descripcion_opiniones.jpg
- **Severidad tentativa:** 2

## Hallazgos - Flujo C

### H7-C
- **Heurística:** H1 - Visibilidad del estado del sistema
- **Pantalla / contexto:** Acciones principales dentro del detalle del producto
- **Descripción:** Aunque el flujo ofrece acciones directas de compra, la jerarquía entre “Agregar al carrito” y otras decisiones previas no siempre deja totalmente claro qué ocurrirá inmediatamente después de pulsar cada opción. Esto puede generar dudas sobre el siguiente paso del proceso.
- **Evidencia:** C1_acciones_compra_producto.jpg
- **Severidad tentativa:** 2

### H8-C
- **Heurística:** H4 - Consistencia y estándares
- **Pantalla / contexto:** Transición desde el producto al carrito
- **Descripción:** El paso desde la evaluación del producto hacia la compra introduce un cambio de contexto importante, pero la interfaz mantiene una alta densidad de información y llamados comerciales que compiten con la tarea principal de avanzar a la compra. Esto reduce la claridad del flujo transaccional.
- **Evidencia:** C2_carrito_resumen.jpg
- **Severidad tentativa:** 2

### H9-C
- **Heurística:** H8 - Estética y diseño minimalista
- **Pantalla / contexto:** Resumen del carrito
- **Descripción:** La pantalla del carrito reúne múltiples bloques de información, mensajes y opciones complementarias, lo que puede distraer al usuario de la acción principal de revisar el pedido y continuar con la compra.
- **Evidencia:** C2_carrito_resumen.jpg
- **Severidad tentativa:** 2

### H10-C
- **Heurística:** H6 - Reconocimiento antes que recuerdo
- **Pantalla / contexto:** Inicio del proceso de compra
- **Descripción:** Al avanzar desde el carrito hacia la compra, el usuario debe integrar mentalmente información que venía revisando en pantallas anteriores, como condiciones, costos y selección del producto. Parte de esa información no siempre aparece resumida con suficiente claridad en el primer paso del checkout.
- **Evidencia:** C3_inicio_proceso_compra.jpg
- **Severidad tentativa:** 2