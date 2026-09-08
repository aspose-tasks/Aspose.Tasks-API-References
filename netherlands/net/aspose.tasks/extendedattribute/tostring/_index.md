---
title: "ExtendedAttribute.ToString"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttribute methode. Retourneert een korte tekenreeksrepresentatie van een uitgebreid attribuut"
type: docs
weight: 110
url: /nl/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

Retourneert een korte tekenreeksrepresentatie van een uitgebreid attribuut.

```csharp
public override string ToString()
```

### Retourwaarde

De tekenreeksrepresentatie van het uitgebreide attribuut.

## Voorbeelden

Toont hoe uitgebreide attributen te lezen.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Lees uitgebreide attributen voor taken
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // lees algemene informatie over uitgebreid attribuut
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### Zie ook

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


