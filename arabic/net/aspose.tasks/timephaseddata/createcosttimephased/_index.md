---
title: CreateCostTimephased
second_title: Aspose.Tasks لمرجع .NET API
description: إنشاء وتهيئة مثيل جديد لملفTimephasedDataaspose.tasks/timephaseddata فئة للبيانات الزمنية على مراحل على أساس التكلفة.
type: docs
weight: 20
url: /ar/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## TimephasedData.CreateCostTimephased method

إنشاء وتهيئة مثيل جديد لملف[`TimephasedData`](../../timephaseddata) فئة للبيانات الزمنية على مراحل على أساس التكلفة.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| uid | Int32 | UID للمهمة. |
| start | DateTime | تاريخ البدء والوقت. |
| finish | DateTime | تاريخ الانتهاء. |
| value | Double | قيمة التكلفة. |
| timeUnit | TimeUnitType | نوع الوحدة الزمنية. |
| type | TimephasedDataType | نوع البيانات الموزعة على الوقت. |

### قيمة الإرجاع

مثال على[`TimephasedData`](../../timephaseddata) فئة للبيانات على مراحل زمنية على أساس التكلفة.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | إذا تم تحديد قيمة تكلفة سلبية. |

### أنظر أيضا

* enum [TimeUnitType](../../timeunittype)
* enum [TimephasedDataType](../../timephaseddatatype)
* class [TimephasedData](../../timephaseddata)
* مساحة الاسم [Aspose.Tasks](../../timephaseddata)
* المجسم [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->