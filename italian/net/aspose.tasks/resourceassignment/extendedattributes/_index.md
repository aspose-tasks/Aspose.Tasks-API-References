---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ResourceAssignment. Ottiene o imposta un'istanza della classe ExtendedAttributeCollection per questo oggetto"
type: docs
weight: 250
url: /it/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

Ottiene o imposta un'istanza della classe ExtendedAttributeCollection per questo oggetto.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## Osservazioni

Lettura supportata solo per il formato XML.

## Esempi

Mostra come aggiungere attributi estesi per un'assegnazione.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Assegna la risorsa "1 TRG: Trade Group" al "TASK 1" creando un oggetto ResourceAssignment.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// Crea una definizione di attributo personalizzato con ricerca.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// Questo valore può essere visualizzato nella vista "Resource usage" di MS Project.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### Vedi anche

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


