---
title: "Aspose::Tasks::Project::GetPageCount метод"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks для C++"
description: "Возвращает количество страниц проекта, которое будет отрисовано, используя масштаб по умолчанию Timescale (Days)."
type: docs
weight: 1090
url: /ru/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Возвращает количество страниц проекта, которое будет отрисовано, используя масштаб по умолчанию Timescale (Days).

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Возвращает количество страниц проекта, который будет отрисован с использованием заданных SaveOptions.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Параметр | Описание |
| --- | --- |
| saveOptions | Параметры сохранения, для которых нужно получить количество страниц. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Возвращает количество страниц для проекта, который будет отрисован с использованием заданных Timescale и PageSize .

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Параметр | Описание |
| --- | --- |
| pageSize | Размер, для которого нужно получить количество страниц. |
| scale | Масштаб, для которого нужно получить количество страниц. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Возвращает количество страниц для проекта, который будет отрисован с использованием заданных Timescale , PresentationFormat и диапазона дат.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Параметр | Описание |
| --- | --- |
| pageSize | Размер, для которого нужно получить количество страниц. |
| scale | Масштаб, для которого нужно получить количество страниц. |
| startDate | Дата начала, для которой нужно получить количество страниц. |
| endDate | Дата окончания, для которой нужно получить количество страниц. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Возвращает количество страниц для проекта, который будет отрисован с использованием Timescale по умолчанию (Days) и заданного PresentationFormat

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Параметр | Описание |
| --- | --- |
| формат | Формат, для которого нужно получить количество страниц. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Возвращает количество страниц для проекта, который будет отрисован с использованием заданных Timescale и PresentationFormat .

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Параметр | Описание |
| --- | --- |
| формат | Формат, для которого нужно получить количество страниц. |
| scale | Масштаб, для которого нужно получить количество страниц. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Возвращает количество страниц для проекта, который будет отрисован с использованием заданного Timescale .

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Параметр | Описание |
| --- | --- |
| scale | Масштаб, для которого нужно получить количество страниц. |

