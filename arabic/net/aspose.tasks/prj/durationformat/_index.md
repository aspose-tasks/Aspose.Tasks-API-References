---
title: "Prj.DurationFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. الصيغة لتعبير عن المدة الإجمالية"
type: docs
weight: 300
url: /ar/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

الصيغة لتعبير عن المدة الإجمالية.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## الأمثلة

يُظهر كيفية قراءة/كتابة خاصية Prj.DurationFormat.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


