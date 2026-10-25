---
title: "تعداد TaskStatus"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.TaskStatus. يحدد حالة المهمة"
type: docs
weight: 2460
url: /ar/net/aspose.tasks/taskstatus/
---
## TaskStatus enumeration

يحدد حالة المهمة.

```csharp
public enum TaskStatus
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | حالة مهمة غير معرفة. |
| Complete | `0` | المهمة مكتملة بنسبة 100٪. |
| OnSchedule | `1` | المهمة في الجدول الزمني إذا كان timephased cumulative percent complete موزع على الأقل حتى اليوم السابق لتاريخ الحالة. |
| Late | `2` | المهمة متأخرة إذا لم يصل timephased cumulative percent complete إلى منتصف الليل في اليوم السابق لتاريخ الحالة. |
| Future | `3` | يتم تعيين حالة المهمة 'Future' عندما يكون تاريخ بدء المهمة أكبر من تاريخ الحالة. |

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


