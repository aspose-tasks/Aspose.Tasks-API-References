---
title: "Rsc.Phonetics"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. التهجئة الصوتية لاسم المورد. للاستخدام مع اللغة اليابانية فقط"
type: docs
weight: 560
url: /ar/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

التهجئة الصوتية لاسم المورد. للاستخدام مع اللغة اليابانية فقط.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.Phonetics.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


