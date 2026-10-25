---
title: "VbaModuleAttribute.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaModuleAttribute methode. Retourneert een hashcode-waarde voor deze VbaModuleAttribute"
type: docs
weight: 40
url: /nl/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

Retourneert een hashcode-waarde voor deze [`VbaModuleAttribute`](../).

```csharp
public override int GetHashCode()
```

### Retourwaarde

Retourneert een hashcode‑waarde voor dit object.

## Voorbeelden

Toont hoe een hashcode van een VBA-module-atribuut te verkrijgen.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// print hashcodes van VBA-module-attributen
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### Zie ook

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


