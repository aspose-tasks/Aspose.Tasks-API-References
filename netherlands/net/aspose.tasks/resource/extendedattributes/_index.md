---
title: "Resource.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource property. Haalt de waarden van een extended attribute op"
type: docs
weight: 320
url: /nl/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

Haalt de waarden van een uitgebreid attribuut op.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Opmerkingen

Twee gegevensstukken zijn nodig - een verwijzing naar de extended attribute-tabel die wordt gespecificeerd ofwel door de unieke ID of het Field ID, en de waarde die wordt gespecificeerd ofwel met de waarde, of een verwijzing naar de waardelijst.

## Voorbeelden

Toont hoe resource extended attributes toe te voegen.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// Definieer extended attribute
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// Maak een uitgebreid attribuut aan en stel de waarde in
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// Voeg een nieuwe resource en het bijbehorende uitgebreide attribuut toe   
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


