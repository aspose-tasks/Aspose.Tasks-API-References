---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition-methode. Retourneert een hashcode voor de instantie van de ExtendedAttributeDefinition-klasse."
type: docs
weight: 330
url: /nl/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

Retourneert een hashcode voor de instantie van de [`ExtendedAttributeDefinition`](../) klasse.

```csharp
public override int GetHashCode()
```

### Retourwaarde

een hashcode voor dit object.

## Voorbeelden

Toont hoe een hashcode van een uitgebreide attribuutdefinitie te verkrijgen.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// de hashcode van een uitgebreide attribuutdefinitie is gelijk aan een veld-id.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### Zie ook

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


