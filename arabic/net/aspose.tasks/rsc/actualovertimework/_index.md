---
title: "Rsc.ActualOvertimeWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. مقدار العمل الإضافي الفعلي الذي تم إنجازه بالفعل من قبل المورد المعين للمهام"
type: docs
weight: 50
url: /ar/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

المقدار الفعلي للعمل الإضافي الذي تم إنجازه بالفعل من قبل المورد المعين للمهام.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


