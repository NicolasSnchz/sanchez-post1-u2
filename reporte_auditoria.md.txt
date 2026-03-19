# Reporte de Auditoría Heurística - Mercado Libre

## 1. Resumen ejecutivo

La presente auditoría heurística evaluó la aplicación móvil **Mercado Libre** en plataforma **Android**, con fecha **19 de marzo de 2026**, tomando como foco tres flujos críticos de uso: **búsqueda y exploración de resultados**, **detalle del producto** y **agregar al carrito e inicio del proceso de compra**. Estos recorridos fueron seleccionados porque representan el trayecto principal de un usuario dentro de una app de comercio electrónico: encontrar un producto, evaluarlo y avanzar hacia la compra.

En total se documentaron **10 hallazgos** de usabilidad, distribuidos entre los tres flujos analizados. El hallazgo más crítico se relaciona con la **sobrecarga visual y competitividad entre elementos comerciales e informativos** dentro de pantallas clave como resultados, detalle del producto y carrito. Este patrón afecta la claridad del recorrido, dificulta la comparación rápida entre opciones y puede generar mayor esfuerzo cognitivo en tareas que deberían resolverse con rapidez.

En términos generales, Mercado Libre ofrece un flujo robusto y funcional, pero la experiencia presenta oportunidades claras de mejora en jerarquía visual, agrupación de información clave y comunicación más explícita del estado del sistema durante tareas de filtrado, evaluación y compra. La principal recomendación es **priorizar el contenido esencial de la tarea sobre mensajes promocionales o bloques secundarios**, para reducir fricción y facilitar decisiones más rápidas y seguras por parte del usuario.

## 2. Metodología

La auditoría se realizó aplicando las **10 heurísticas de Nielsen** sobre una aplicación móvil real instalada en un dispositivo Android. El proceso consistió en definir previamente el alcance de la evaluación, seleccionar tres flujos principales y recorrerlos de manera estructurada para identificar posibles violaciones heurísticas.

Los flujos evaluados fueron los siguientes:  
**Flujo A:** búsqueda de producto y exploración de resultados.  
**Flujo B:** detalle del producto.  
**Flujo C:** agregar al carrito e inicio del proceso de compra.

La evaluación se apoyó en observación directa de la interfaz y en la captura de evidencia visual mediante pantallazos organizados en la carpeta `evidencias/`. Cada hallazgo fue registrado en `checklist_heuristico.md` con los seis campos requeridos: ID, heurística, pantalla o contexto, descripción del problema, evidencia y severidad tentativa. Posteriormente, se revisaron los hallazgos de manera conjunta para consolidar una priorización final según impacto percibido en la experiencia de usuario.

El enfoque de análisis no se centró en errores técnicos de funcionamiento, sino en problemas relacionados con **claridad, consistencia, carga cognitiva, jerarquía visual y comprensión del flujo**.

## 3. Hallazgos por flujo

### Flujo A: búsqueda y exploración de resultados

En este flujo se identificaron tres hallazgos principales.  
El primero corresponde a la pantalla de resultados de búsqueda, donde existe una **alta densidad de información por tarjeta**, con múltiples etiquetas, promociones, precios, cuotas y mensajes simultáneos. Esto reduce la escaneabilidad del contenido y dificulta comparar productos con rapidez. Evidencia: `A1_resultados_busqueda.jpg`.

El segundo hallazgo se observó tras aplicar filtros. Aunque la lista cambia, la interfaz no siempre comunica de forma suficientemente explícita qué criterio quedó activo ni cuál fue el efecto exacto sobre los resultados. Esto puede generar incertidumbre en el usuario. Evidencia: `A2_resultados_filtrados.jpg`.

El tercer hallazgo aparece en la exploración refinada de resultados, donde controles, etiquetas comerciales y elementos informativos comparten protagonismo visual, afectando la identificación inmediata de las acciones principales del flujo. Evidencia: `A3_resultados_ordenados.jpg`.

### Flujo B: detalle del producto

En la parte superior del detalle del producto se identificó una **sobrecarga visual** derivada de la concentración de imagen, precio, descuentos, cuotas, promociones y etiquetas comerciales en un mismo bloque. Esto dificulta reconocer con rapidez qué información es la más importante para decidir si continuar con el producto. Evidencia: `B1_detalle_producto_superior.jpg`.

También se observó que la información clave para tomar decisiones, como envío, reputación del vendedor, condiciones y confianza, aparece distribuida en bloques separados, lo que obliga al usuario a recordar datos vistos antes para integrarlos mentalmente. Evidencia: `B2_envio_vendedor_condiciones.jpg`.

Finalmente, en secciones como descripción, opiniones o información técnica, la interfaz no siempre deja claro qué contenido es prioritario dentro del recorrido de evaluación. La información relevante está dispersa a lo largo de un desplazamiento extenso. Evidencia: `B3_descripcion_opiniones.jpg`.

### Flujo C: agregar al carrito e inicio del proceso de compra

En la zona de acciones principales del producto, la jerarquía entre decisiones como “Agregar al carrito” y otras acciones de compra no siempre deja completamente claro qué ocurrirá inmediatamente después de pulsarlas. Evidencia: `C1_acciones_compra_producto.jpg`.

En la transición hacia el carrito se presenta un cambio de contexto importante, pero siguen apareciendo bloques y estímulos visuales que compiten con la tarea principal de revisar el pedido y continuar con la compra. Evidencia: `C2_carrito_resumen.jpg`.

En el carrito se evidenció nuevamente una concentración de bloques, mensajes y opciones complementarias que pueden distraer de la acción principal. Además, al avanzar al inicio del proceso de compra, parte de la información revisada en pantallas anteriores no siempre aparece resumida con suficiente claridad. Evidencia: `C2_carrito_resumen.jpg` y `C3_inicio_proceso_compra.jpg`.

## 4. Tabla de priorización consolidada

| Prioridad | ID | Heurística | Severidad final | Impacto en usuario | Recomendación |
|---|---|---|---:|---|---|
| 1 | H4-B | H8 - Estética y diseño minimalista | 3 | La sobrecarga visual en el detalle del producto dificulta identificar la información principal para decidir. | Reducir la competencia visual entre promociones y contenido clave, priorizando precio, nombre, disponibilidad y atributos esenciales. |
| 2 | H1-A | H8 - Estética y diseño minimalista | 3 | La comparación rápida entre productos se vuelve más difícil por la densidad de información en resultados. | Simplificar la tarjeta de producto y jerarquizar mejor descuentos, cuotas y envío. |
| 3 | H9-C | H8 - Estética y diseño minimalista | 3 | El carrito pierde claridad como paso transaccional por exceso de bloques y mensajes secundarios. | Limitar elementos no esenciales dentro del carrito y resaltar el resumen del pedido y la acción principal. |
| 4 | H5-B | H6 - Reconocimiento antes que recuerdo | 2 | El usuario debe integrar mentalmente información dispersa para evaluar la compra. | Agrupar envío, reputación, condiciones y datos de confianza en un bloque más unificado. |
| 5 | H10-C | H6 - Reconocimiento antes que recuerdo | 2 | El inicio del checkout no resume con suficiente claridad toda la información necesaria para continuar con seguridad. | Mostrar un resumen más claro del producto, costos y condiciones al entrar al proceso de compra. |
| 6 | H2-A | H1 - Visibilidad del estado del sistema | 2 | Puede haber duda sobre qué filtro quedó activo y cómo afectó los resultados. | Hacer más visible el estado de los filtros aplicados mediante chips o etiquetas persistentes. |
| 7 | H6-B | H1 - Visibilidad del estado del sistema | 2 | La información prioritaria no siempre es evidente dentro del recorrido largo del detalle. | Reorganizar el detalle para destacar primero el contenido más útil para decidir. |
| 8 | H7-C | H1 - Visibilidad del estado del sistema | 2 | La acción de compra puede no comunicar con total claridad la consecuencia inmediata del toque. | Diferenciar mejor los resultados esperados de cada botón principal. |
| 9 | H3-A | H4 - Consistencia y estándares | 2 | La mezcla de controles y etiquetas comerciales reduce la claridad del flujo de búsqueda. | Unificar visualmente controles de refinamiento y separar promociones del contenido funcional. |
| 10 | H8-C | H4 - Consistencia y estándares | 2 | La transición al carrito mantiene estímulos visuales que compiten con la tarea principal. | Reforzar una vista más limpia y enfocada al revisar el pedido antes de continuar. |

## 5. Análisis de patrones

El primer patrón recurrente identificado es la **sobrecarga visual en pantallas críticas**, especialmente en resultados, detalle del producto y carrito. En varios puntos del recorrido, la app combina demasiados elementos comerciales, etiquetas promocionales, mensajes de valor y bloques informativos al mismo tiempo. Esto genera una interfaz funcional, pero poco minimalista en términos heurísticos, afectando la velocidad de lectura y la claridad del recorrido.

El segundo patrón es la **dispersión de información clave para la toma de decisiones**. En el detalle del producto y en el inicio del proceso de compra, el usuario necesita integrar mentalmente información que se encuentra separada en distintas secciones o pantallas. En lugar de reconocer de inmediato lo más importante, debe recordar y reconstruir el contexto, lo que incrementa el esfuerzo cognitivo.

Como patrón complementario, también se observó una **comunicación mejorable del estado del sistema** en acciones como aplicar filtros o pasar de una etapa a otra dentro del flujo de compra. Aunque la app sí responde, no siempre comunica con la máxima claridad qué cambió o qué ocurrirá a continuación.

## 6. Conclusiones

La aplicación Mercado Libre presenta una experiencia madura, amplia y funcional, alineada con su propósito comercial y con un flujo general entendible para la mayoría de los usuarios. Sin embargo, desde la perspectiva heurística, existen oportunidades claras de mejora relacionadas con la claridad visual, la organización de la información y la reducción de carga cognitiva en tareas de exploración y compra.

Los hallazgos obtenidos muestran que la app no falla principalmente por ausencia de funciones, sino por la forma en que múltiples elementos compiten dentro de la misma pantalla. Esto afecta sobre todo los momentos de comparación, evaluación y decisión, que son precisamente los más críticos dentro de una experiencia de e-commerce.

Como conclusión general, la app cumple su objetivo, pero podría mejorar considerablemente si reduce ruido visual, agrupa mejor la información esencial y fortalece la visibilidad del estado del sistema en los puntos donde el usuario cambia de contexto. Las recomendaciones prioritarias son: simplificar resultados, reorganizar el detalle del producto y hacer más claro el resumen informativo al inicio del proceso de compra.