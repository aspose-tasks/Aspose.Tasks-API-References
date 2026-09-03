---
title: "Aspose::Tasks::Project::GetPageCount methode"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks voor C++"
description: "Retourneert het aantal pagina's voor het project dat wordt gerenderd met de standaard Timescale (Days)."
type: docs
weight: 1090
url: /nl/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Retourneert het aantal pagina's voor het project dat wordt gerenderd met de standaard Timescale (Days).

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Retourneert het paginacount voor het project dat wordt gerenderd met de opgegeven SaveOptions.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Parameter | Beschrijving |
| --- | --- |
| saveOptions | De opslaanopties om het paginacount te verkrijgen. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven Timescale en PageSize.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Parameter | Beschrijving |
| --- | --- |
| pageSize | De grootte om de paginatelling voor te krijgen. |
| scale | De schaal om de paginatelling voor te krijgen. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven Timescale, PresentationFormat en datumbereik.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Parameter | Beschrijving |
| --- | --- |
| pageSize | De grootte om de paginatelling voor te krijgen. |
| scale | De schaal om de paginatelling voor te krijgen. |
| startDate | De startdatum om de paginatelling voor te krijgen. |
| endDate | De einddatum om de paginatelling voor te krijgen. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Retourneert paginatelling voor het project dat wordt gerenderd met de standaard Timescale (Days) en de opgegeven PresentationFormat.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Parameter | Beschrijving |
| --- | --- |
| indeling | Het formaat om de paginatelling voor te krijgen. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven Timescale en PresentationFormat.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Parameter | Beschrijving |
| --- | --- |
| indeling | Het formaat om de paginatelling voor te krijgen. |
| scale | De schaal om de paginatelling voor te krijgen. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Retourneert paginatelling voor het project dat wordt gerenderd met de opgegeven Timescale.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Parameter | Beschrijving |
| --- | --- |
| scale | De schaal om de paginatelling voor te krijgen. |

