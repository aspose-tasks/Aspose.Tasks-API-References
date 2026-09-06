---
title: "Rsc.RemainingWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. الوقت المتبقي المطلوب لإكمال مهمة أو مجموعة مهام"
type: docs
weight: 610
url: /ar/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

الوقت المتبقي المطلوب لإكمال مهمة أو مجموعة مهام.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


