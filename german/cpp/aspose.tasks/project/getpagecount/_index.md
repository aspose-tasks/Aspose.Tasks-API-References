---
title: "Aspose::Tasks::Project::GetPageCount Methode"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks für C++"
description: "Gibt die Seitenanzahl für das Projekt zurück, das mit der Standard Timescale (Days) gerendert wird."
type: docs
weight: 1090
url: /de/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Gibt die Seitenanzahl für das Projekt zurück, das mit der Standard Timescale (Days) gerendert wird.

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Gibt die Seitenzahl für das Projekt zurück, das mit den angegebenen SaveOptions gerendert werden soll.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Parameter | Beschreibung |
| --- | --- |
| saveOptions | Die Speicheroptionen, um die Seitenzahl zu erhalten. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Gibt die Seitenzahl für das Projekt zurück, das mit der angegebenen Timescale und PageSize gerendert wird.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Parameter | Beschreibung |
| --- | --- |
| pageSize | Die Größe, um die Seitenzahl zu erhalten. |
| scale | Der Maßstab, um die Seitenzahl zu erhalten. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Gibt die Seitenzahl für das Projekt zurück, das mit der angegebenen Timescale, PresentationFormat und dem Datumsbereich gerendert wird.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Parameter | Beschreibung |
| --- | --- |
| pageSize | Die Größe, um die Seitenzahl zu erhalten. |
| scale | Der Maßstab, um die Seitenzahl zu erhalten. |
| startDate | Das Startdatum, um die Seitenzahl zu erhalten. |
| endDate | Das Enddatum, um die Seitenzahl zu erhalten. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Gibt die Seitenzahl für das Projekt zurück, das mit der Standard‑Timescale (Tage) und dem angegebenen PresentationFormat gerendert wird

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Parameter | Beschreibung |
| --- | --- |
| format | Das Format, um die Seitenzahl zu erhalten. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Gibt die Seitenzahl für das Projekt zurück, das mit der angegebenen Timescale und PresentationFormat gerendert wird.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Parameter | Beschreibung |
| --- | --- |
| format | Das Format, um die Seitenzahl zu erhalten. |
| scale | Der Maßstab, um die Seitenzahl zu erhalten. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Gibt die Seitenzahl für das Projekt zurück, das mit der angegebenen Timescale gerendert wird.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Parameter | Beschreibung |
| --- | --- |
| scale | Der Maßstab, um die Seitenzahl zu erhalten. |

