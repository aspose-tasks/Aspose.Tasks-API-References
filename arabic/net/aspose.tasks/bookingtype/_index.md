---
title: "التعداد BookingType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.BookingType. يحدد نوع الحجز لمورد."
type: docs
weight: 150
url: /ar/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

يحدد نوع الحجز لمورد.

```csharp
public enum BookingType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | يشير إلى أن القيمة لم تُحدد في ملف المشروع الأصلي. |
| Committed | `0` | يشير إلى نوع الحجز المُلتزم. |
| Proposed | `1` | يشير إلى نوع الحجز المقترح. |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Asn.BookingType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


