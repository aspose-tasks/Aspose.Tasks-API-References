---
title: "Rsc.ActualWorkProtected"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. مقدار العمل الذي يتم من خلاله حماية العمل الفعلي"
type: docs
weight: 80
url: /ar/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

المقدار الذي يتم من خلاله حماية العمل الفعلي.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


