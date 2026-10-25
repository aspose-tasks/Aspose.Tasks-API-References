---
title: "Rsc.ActualWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. مقدار العمل الذي تم إنجازه بالفعل من قبل المورد المعين للمهام"
type: docs
weight: 70
url: /ar/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

المقدار الذي تم إنجازه بالفعل من قبل المورد المعين للمهام.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


