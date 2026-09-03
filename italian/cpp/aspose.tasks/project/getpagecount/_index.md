---
title: "Aspose::Tasks::Project::GetPageCount metodo"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks per C++"
description: "Restituisce il conteggio delle pagine per il progetto da renderizzare usando la Timescale predefinita (Giorni)."
type: docs
weight: 1090
url: /it/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Restituisce il conteggio delle pagine per il progetto da renderizzare usando la Timescale predefinita (Giorni).

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Restituisce il conteggio delle pagine per il progetto da renderizzare utilizzando le SaveOptions specificate.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Parametro | Descrizione |
| --- | --- |
| saveOptions | Le opzioni di salvataggio per le quali ottenere il conteggio delle pagine. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Restituisce il conteggio delle pagine per il progetto da rendere usando il Timescale e la PageSize forniti.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Parametro | Descrizione |
| --- | --- |
| pageSize | La dimensione per cui ottenere il conteggio delle pagine. |
| scale | La scala per cui ottenere il conteggio delle pagine. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Restituisce il conteggio delle pagine per il progetto da rendere usando il Timescale, il PresentationFormat e l'intervallo di date forniti.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Parametro | Descrizione |
| --- | --- |
| pageSize | La dimensione per cui ottenere il conteggio delle pagine. |
| scale | La scala per cui ottenere il conteggio delle pagine. |
| startDate | La data di inizio per cui ottenere il conteggio delle pagine. |
| endDate | La data di fine per cui ottenere il conteggio delle pagine. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Restituisce il conteggio delle pagine per il progetto da rendere usando il Timescale predefinito (Giorni) e il PresentationFormat fornito.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Parametro | Descrizione |
| --- | --- |
| formato | Il formato per cui ottenere il conteggio delle pagine. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Restituisce il conteggio delle pagine per il progetto da rendere usando il Timescale e il PresentationFormat forniti.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Parametro | Descrizione |
| --- | --- |
| formato | Il formato per cui ottenere il conteggio delle pagine. |
| scale | La scala per cui ottenere il conteggio delle pagine. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Restituisce il conteggio delle pagine per il progetto da rendere usando il Timescale fornito.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Parametro | Descrizione |
| --- | --- |
| scale | La scala per cui ottenere il conteggio delle pagine. |

