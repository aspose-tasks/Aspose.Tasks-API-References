---
title: "Rsc.RemainingOvertimeWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. مقدار الوقت الإضافي المجدول المتبقي"
type: docs
weight: 600
url: /ar/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

مقدار العمل الإضافي المجدول المتبقي.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


