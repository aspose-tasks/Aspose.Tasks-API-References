---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment‑eigenschap. Haalt een instantie op of stelt deze in van de klasse ExtendedAttributeCollection voor dit object."
type: docs
weight: 250
url: /nl/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

Geeft of stelt een instantie van de ExtendedAttributeCollection class voor dit object in.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## Opmerkingen

Lezen wordt alleen ondersteund voor XML-indeling.

## Voorbeelden

Toont hoe uitgebreide attributen toe te voegen voor een toewijzing.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Wijs resource "1 TRG: Trade Group" toe aan "TASK 1" door een ResourceAssignment-object te maken.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// Maak een aangepaste attribuutdefinitie met zoekopdracht.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// Deze waarde is te zien in de weergave "Resource usage" van MS Project.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### Zie ook

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


