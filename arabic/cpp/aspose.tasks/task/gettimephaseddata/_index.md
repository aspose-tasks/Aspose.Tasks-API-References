---
title: "Aspose::Tasks::Task::GetTimephasedData طريقة"
linktitle: "GetTimephasedData"
articleTitle: "GetTimephasedData"
second_title: "Aspose.Tasks لـ C++"
description: "يرجع كائن TimephasedDataCollection مع قيم TimephasedData ضمن تواريخ البدء والانتهاء المحددة."
type: docs
weight: 1360
url: /ar/cpp/aspose.tasks/task/gettimephaseddata/
---

## GetTimephasedData (1 of 2) {#gettimephaseddata_1}

يرجع كائن TimephasedDataCollection مع قيم TimephasedData ضمن تواريخ البدء والانتهاء المحددة.

**Returns:** List of Aspose::Tasks::TimephasedData to be filled in.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end)
```

| معامل | الوصف |
| --- | --- |
| بدء | تاريخ البدء لبيانات الوقت المرحلية. |
| end | تاريخ الانتهاء لبيانات الوقت المرحلية. |

---

## GetTimephasedData (2 of 2) {#gettimephaseddata_2}

يرجع كائن TimephasedDataCollection مع قيم TimephasedData ضمن تواريخ البدء والنهاية المحددة لنوع البيانات المرحلية المحدد.

**Returns:** A TimephasedDataCollection object with TimephasedData values within given start and end dates of specified timephased data type.

```cpp
GetTimephasedData(System::DateTime start, System::DateTime end, TimephasedDataType timephasedType)
```

| معامل | الوصف |
| --- | --- |
| بدء | تاريخ البدء لبيانات الوقت المرحلية. |
| end | تاريخ الانتهاء لبيانات الوقت المرحلية. |
| timephasedType | نوع بيانات الوقت المرحلية ( Aspose::Tasks::TimephasedDataType ). |

