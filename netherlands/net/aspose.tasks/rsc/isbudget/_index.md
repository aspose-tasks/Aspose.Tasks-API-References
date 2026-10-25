---
title: "Rsc.IsBudget"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Bepaalt of een werkmateriaal- of kostresource een budgetresource is"
type: docs
weight: 380
url: /nl/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

Bepaalt of een werk‑, materiaal‑ of kostenresource een budgetresource is.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.IsBudget te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


