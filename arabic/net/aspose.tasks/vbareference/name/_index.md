---
title: "VbaReference.Name"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaReference. تحصل أو تعين اسم مرجع VBA"
type: docs
weight: 30
url: /ar/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

يحصل أو يعيّن اسم مرجع VBA.

```csharp
public string Name { get; set; }
```

## الأمثلة

يوضح كيفية قراءة مراجع VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### انظر أيضًا

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


