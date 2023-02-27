---
title: TimephasedData.CreateWorkTimephased
second_title: Aspose.Tasks لمرجع .NET API
description: TimephasedData طريقة. إنشاء مثيل جديد لملفTimephasedData فئة للبيانات على مراحل الوقت المستندة إلى العمل .
type: docs
weight: 40
url: /ar/net/aspose.tasks/timephaseddata/createworktimephased/
---
## TimephasedData.CreateWorkTimephased method

إنشاء مثيل جديد لملف[`TimephasedData`](../) فئة للبيانات على مراحل الوقت المستندة إلى العمل .

```csharp
public static TimephasedData CreateWorkTimephased(int uid, DateTime start, DateTime finish, 
    TimeSpan value, TimeUnitType timeUnit, TimephasedDataType type)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| uid | Int32 | UID للمهمة. |
| start | DateTime | تاريخ البدء والوقت. |
| finish | DateTime | تاريخ الانتهاء. |
| value | TimeSpan | قيمة الوقت. |
| timeUnit | TimeUnitType | نوع الوحدة الزمنية. |
| type | TimephasedDataType | نوع البيانات الموزعة على الوقت. |

### قيمة الإرجاع

مثال على[`TimephasedData`](../) فئة للبيانات القائمة على الوقت على مراحل.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | إذا تم تحديد قيمة عمل سالبة. |

### أنظر أيضا

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* مساحة الاسم [Aspose.Tasks](../../timephaseddata/)
* المجسم [Aspose.Tasks](../../../)


