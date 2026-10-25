---
title: "ExtendedAttributeDefinition.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition-methode. Retourneert een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object"
type: docs
weight: 320
url: /nl/net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

Retourneert een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | het opgegeven object om te vergelijken met deze instantie. |

### Retourwaarde

een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object.

## Voorbeelden

Toont hoe de gelijkheid van een uitgebreide attribuutdefinitie te controleren.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// de gelijkheid van kalenders wordt gecontroleerd ten opzichte van de veld-id's van de attribuutdefinitie.
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### Zie ook

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


