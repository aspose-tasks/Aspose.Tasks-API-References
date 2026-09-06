---
title: "الفئة VbaReferenceCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.VbaReferenceCollection. تمثل مجموعة من كائنات VbaReference"
type: docs
weight: 2880
url: /ar/net/aspose.tasks/vbareferencecollection/
---
## VbaReferenceCollection class

تمثل مجموعة من كائنات [`VbaReference`](../vbareference/).

```csharp
public class VbaReferenceCollection : ReadOnlyCollectionBase<VbaReference>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaReference) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## الأمثلة

يعرض كيفية العمل مع مجموعة مراجع VBA.

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

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaReference](../vbareference/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


