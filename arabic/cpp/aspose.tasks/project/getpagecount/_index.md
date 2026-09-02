---
title: "Aspose::Tasks::Project::GetPageCount طريقة"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks لـ C++"
description: "يعيد عدد الصفحات للمشروع ليتم عرضه باستخدام مقياس الوقت الافتراضي (Days)."
type: docs
weight: 1090
url: /ar/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

يعيد عدد الصفحات للمشروع ليتم عرضه باستخدام مقياس الوقت الافتراضي (Days).

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

يعيد عدد الصفحات للمشروع ليتم عرضه باستخدام خيارات الحفظ المحددة.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| معامل | الوصف |
| --- | --- |
| saveOptions | خيارات الحفظ للحصول على عدد الصفحات. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

يعيد عدد الصفحات للمشروع ليتم عرضه باستخدام المقياس الزمني وحجم الصفحة المحددين.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| معامل | الوصف |
| --- | --- |
| pageSize | الحجم للحصول على عدد الصفحات. |
| scale | المقياس للحصول على عدد الصفحات. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام المقياس الزمني المحدد ، تنسيق العرض والفترة الزمنية.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| معامل | الوصف |
| --- | --- |
| pageSize | الحجم للحصول على عدد الصفحات. |
| scale | المقياس للحصول على عدد الصفحات. |
| startDate | تاريخ البدء للحصول على عدد الصفحات. |
| endDate | تاريخ الانتهاء للحصول على عدد الصفحات. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام المقياس الزمني الافتراضي (أيام) وتنسيق العرض المحدد

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| معامل | الوصف |
| --- | --- |
| تنسيق | التنسيق للحصول على عدد الصفحات. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام المقياس الزمني المحدد وتنسيق العرض.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| معامل | الوصف |
| --- | --- |
| تنسيق | التنسيق للحصول على عدد الصفحات. |
| scale | المقياس للحصول على عدد الصفحات. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام المقياس الزمني المحدد.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| معامل | الوصف |
| --- | --- |
| scale | المقياس للحصول على عدد الصفحات. |

