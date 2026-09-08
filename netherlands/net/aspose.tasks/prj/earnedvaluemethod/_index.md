---
title: "Prj.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De standaardmethode voor het berekenen van verdiende waarde"
type: docs
weight: 310
url: /nl/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

De standaardmethode voor het berekenen van verdiende waarde.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## Voorbeelden

Toont hoe de eigenschap Prj.EarnedValueMethod te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


