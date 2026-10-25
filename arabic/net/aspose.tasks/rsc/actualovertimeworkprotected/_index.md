---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Rsc field. كمية العمل التي يتم من خلالها حماية العمل الإضافي الفعلي"
type: docs
weight: 60
url: /ar/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

المقدار الذي يتم من خلاله حماية العمل الإضافي الفعلي.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Rsc.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


