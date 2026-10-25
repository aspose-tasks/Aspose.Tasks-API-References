---
title: "VbaProject.References"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaProject. تحصّل على مجموعة من VbaReferenceCollection"
type: docs
weight: 70
url: /ar/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

تحصّل على مجموعة من [`VbaReferenceCollection`](../../vbareferencecollection/)

```csharp
public VbaReferenceCollection References { get; }
```

## الأمثلة

يظهر كيفية قراءة معلومات مراجع مشروع VBA.

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

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


