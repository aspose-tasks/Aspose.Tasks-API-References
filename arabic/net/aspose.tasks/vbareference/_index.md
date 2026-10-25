---
title: "الفئة VbaReference"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.VbaReference. تمثل مرجعًا لمشروع VbaProject"
type: docs
weight: 2870
url: /ar/net/aspose.tasks/vbareference/
---
## VbaReference class

يمثل مرجعًا لـ [`VbaProject`](../vbaproject/).

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [VbaReference](vbareference/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | يحصل على معرف المكتبة. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | يحصل أو يعيّن اسم مرجع VBA. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | يرجع قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن `VbaReference` المحدد. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | يرجع قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن `VbaReference` المحدد. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | يرجع قيمة رمز تجزئة لهذا `VbaReference`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


