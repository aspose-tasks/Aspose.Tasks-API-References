---
title: "طريقة Aspose::Tasks::ResourceAssignment::GetTimephasedData"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks لـ C++"
description: "يعيد كائن TimephasedDataCollection مع نسخ الفئة TimephasedData ضمن تواريخ البدء والانتهاء المحددة لـ TimephasedDataType::AssignmentWork."
type: docs
weight: 720
url: /ar/cpp/aspose.tasks/resourceassignment/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

يعيد كائن TimephasedDataCollection مع نسخ الفئة TimephasedData ضمن تواريخ البدء والانتهاء المحددة لـ TimephasedDataType::AssignmentWork.

**Returns:** returns a list containing instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| معامل | الوصف |
| --- | --- |
| بدء | تاريخ البدء لبيانات الوقت المرحلية. |
| end | تاريخ الانتهاء لبيانات الوقت المرحلية. |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

يعيد كائن الفئة TimephasedDataCollection الذي يحتوي على كائنات الفئة TimephasedData ضمن تواريخ البدء والنهاية المحددة لنوع TimephasedDataType

**Returns:** returns a list which contains instances of Aspose::Tasks::TimephasedData class.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| معامل | الوصف |
| --- | --- |
| بدء | تاريخ البدء لبيانات الوقت المرحلية. |
| end | تاريخ الانتهاء لبيانات الوقت المرحلية. |
| timephasedType | نوع بيانات الوقت المرحلية ( Aspose::Tasks::TimephasedDataType ). |

