---
title: "Prj.AreEditableActualCosts"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Gerçek maliyetlerin düzenlenebilir olup olmadığını belirler"
type: docs
weight: 30
url: /tr/net/aspose.tasks/prj/areeditableactualcosts/
---
## Prj.AreEditableActualCosts field

Gerçek maliyetlerin düzenlenebilir olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> AreEditableActualCosts;
```

## Örnekler

Prj.AreEditableActualCosts özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.AreEditableActualCosts, true);

Console.WriteLine("Are Editable Actual Costs: " + project.Get(Prj.AreEditableActualCosts));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


