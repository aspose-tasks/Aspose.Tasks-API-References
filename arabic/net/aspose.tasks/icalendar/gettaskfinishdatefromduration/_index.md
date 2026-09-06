---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ICalendar. تحسب تاريخ وانتهاء المهمة والوقت من أجزاء تاريخ البدء المقسمة ومدة العمل"
type: docs
weight: 50
url: /ar/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

يحسب تاريخ ووقت انتهاء المهمة من تاريخ بدايتها، الأجزاء المقسمة ومدة العمل.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| مهمة | مهمة | المهمة لحساب تاريخ الانتهاء لها. |
| المدة | TimeSpan | المدة التي سيتم حسابها. |

### قيمة الإرجاع

تاريخ انتهاء المهمة لتاريخ البدء والمدة المحددين.

## ملاحظات

يرجع DateTime.MinValue إذا كانت المهمة ملخصًا، أو null أو إذا لم يتم تعيين تاريخ البدء الخاص بها.

### انظر أيضًا

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


