---
title: "Rsc.Work"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. إجمالي مقدار الوقت المجدول لمورد على مهمة"
type: docs
weight: 690
url: /ar/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

إجمالي مقدار الوقت المجدول للمورد على مهمة.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


