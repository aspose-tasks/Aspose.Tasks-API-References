---
title: "Aspose::Tasks::Project::GetPageCount método"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks for C++"
description: "Devuelve el recuento de páginas del proyecto que se renderizará usando la escala de tiempo predeterminada (Días)."
type: docs
weight: 1090
url: /es/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Devuelve el recuento de páginas del proyecto que se renderizará usando la escala de tiempo predeterminada (Días).

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Devuelve el recuento de páginas del proyecto que se renderizará usando las SaveOptions proporcionadas.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Parámetro | Descripción |
| --- | --- |
| saveOptions | Las opciones de guardado para obtener el recuento de páginas. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Devuelve el recuento de páginas del proyecto que se renderizará usando la Timescale y PageSize .

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Parámetro | Descripción |
| --- | --- |
| pageSize | El tamaño para obtener el recuento de páginas. |
| scale | La escala para obtener el recuento de páginas. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Devuelve el recuento de páginas del proyecto que se renderizará usando la Timescale, PresentationFormat y el rango de fechas.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Parámetro | Descripción |
| --- | --- |
| pageSize | El tamaño para obtener el recuento de páginas. |
| scale | La escala para obtener el recuento de páginas. |
| startDate | La fecha de inicio para obtener el recuento de páginas. |
| endDate | La fecha de fin para obtener el recuento de páginas. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Devuelve el recuento de páginas del proyecto que se renderizará usando la Timescale predeterminada (Days) y la PresentationFormat proporcionada.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Parámetro | Descripción |
| --- | --- |
| formato | El formato para obtener el recuento de páginas. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Devuelve el recuento de páginas del proyecto que se renderizará usando la Timescale y PresentationFormat .

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Parámetro | Descripción |
| --- | --- |
| formato | El formato para obtener el recuento de páginas. |
| scale | La escala para obtener el recuento de páginas. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Devuelve el recuento de páginas del proyecto que se renderizará usando la Timescale .

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Parámetro | Descripción |
| --- | --- |
| scale | La escala para obtener el recuento de páginas. |

