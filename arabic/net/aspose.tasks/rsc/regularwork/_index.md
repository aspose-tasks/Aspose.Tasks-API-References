---
title: "Rsc.RegularWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. إجمالي مقدار العمل غير الإضافي المجدول للقيام به من قبل المورد"
type: docs
weight: 570
url: /ar/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

إجمالي مقدار العمل غير الإضافي المجدول الذي سيؤديه المورد.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


