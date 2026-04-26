# Auditoría de trazabilidad — Paso 11: Pseudocódigo del Sistema

Documento auditado: `11-pseudocodigo-sistema.md`
Sección: "Ejemplo correcto con Cerrajeros Madrid 24h" (dentro de cada bloque del pseudocódigo)
Negocio: Cerrajeros Madrid 24h

---

## A. Cobertura añadida (1 decisión)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 11.01 | Se añade una 5ª Local Coverage Area no mencionada en pasos previos | Centro |

---

## B. Cambio de página ejemplo (1 decisión)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 11.02 | Se elige una nueva LBS de ejemplo distinta a la del paso 3/9 | LBS-001 = `/cerrajero/madrid/apertura-puertas/` |

---

## C. Reformulación de GeoArticle (2 decisiones)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 11.03 | Se reformula el título del GeoArticle de costes | "¿Cuánto cuesta un cerrajero urgente en Madrid?" |
| 11.04 | Se reformula la URL del GeoArticle de costes | `/madrid/cuanto-cuesta-un-cerrajero-urgente/` |

---

## D. Anchors para nuevo LBS (1 decisión)

| ID | Decisión tomada | Valor decidido en el ejemplo |
|---|---|---|
| 11.05 | Anchors para el LBS apertura-puertas | "apertura de puertas en Madrid", "servicios de cerrajería en Madrid", "cerrajero urgente en Madrid" |

---

**Total decisiones detectadas en el paso 11: 5**

**Distribución por bloque:**
- A. Cobertura añadida: 1
- B. Cambio de página ejemplo: 1
- C. Reformulación de GeoArticle: 2
- D. Anchors para nuevo LBS: 1

**Notas (inconsistencias importantes):**
- En paso 1 las Local Coverage Areas son 4 (Almagro, Chamberí, Salamanca, Retiro). En paso 11 aparecen 5 (se añade Centro) sin justificación.
- En paso 4 el GeoArticle de costes se llama `guia-precios-cerrajero-urgente`. En paso 11 se llama `cuanto-cuesta-un-cerrajero-urgente`. Misma intención, dos slugs distintos.
- El LBS ejemplo cambia de `/cerrajero/madrid/cerrajero-urgente/` (pasos 3, 6, 7, 9) a `/cerrajero/madrid/apertura-puertas/` (paso 11).
- En paso 1 hay 5 servicios core. En paso 11 línea 261 aparece "Duplicado de llaves" listado como core service, en conflicto con la clasificación previa de "Duplicado de llaves" como categoría adicional con página propia.
