---
title: "الفئة VbaModuleAttributeCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.VbaModuleAttributeCollection. تمثّل مجموعة من كائنات VbaModuleAttribute."
type: docs
weight: 2830
url: /ar/net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

تمثّل مجموعة من كائنات [`VbaModuleAttribute`](../vbamoduleattribute/).

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## الأمثلة

يظهر كيفية التكرار عبر مجموعة سمات وحدة VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("Attribute Name: " + attribute.Key);
        Console.WriteLine("Attribute Value: " + attribute.Value);
    }
}
```

### انظر أيضًا

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


