---
title: "VbaReference.LibIdentifier"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaReference. يحصل على معرف المكتبة"
type: docs
weight: 20
url: /ar/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

يحصل على معرف المكتبة.

```csharp
public string LibIdentifier { get; }
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


