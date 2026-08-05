---
title: "Aspose::Tasks::Project::GetPageCount method"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks for C++"
description: "Returns page count for the project to be rendered using default Timescale (Days)."
type: docs
weight: 1090
url: /cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Returns page count for the project to be rendered using default Timescale (Days).

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Returns page count for the project to be rendered using given SaveOptions .

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Parameter | Description |
| --- | --- |
| saveOptions | The save options to get page count for. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Returns page count for the project to be rendered using given Timescale and PageSize .

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Parameter | Description |
| --- | --- |
| pageSize | The size to get page count for. |
| scale | The scale to get page count for. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Returns page count for the project to be rendered using given Timescale , PresentationFormat and date range.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Parameter | Description |
| --- | --- |
| pageSize | The size to get page count for. |
| scale | The scale to get page count for. |
| startDate | The start date to get page count for. |
| endDate | The end date to get page count for. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Returns page count for the project to be rendered using default Timescale (Days) and given PresentationFormat

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Parameter | Description |
| --- | --- |
| format | The format to get page count for. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Returns page count for the project to be rendered using given Timescale and PresentationFormat .

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Parameter | Description |
| --- | --- |
| format | The format to get page count for. |
| scale | The scale to get page count for. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Returns page count for the project to be rendered using given Timescale .

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Parameter | Description |
| --- | --- |
| scale | The scale to get page count for. |

