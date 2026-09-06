---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ResourceAssignment. Obtient ou définit une instance de la classe ExtendedAttributeCollection pour cet objet."
type: docs
weight: 250
url: /fr/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

Obtient ou définit une instance de la classe ExtendedAttributeCollection pour cet objet.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## Remarques

Lecture prise en charge uniquement au format XML.

## Exemples

Montre comment ajouter des attributs étendus pour une affectation.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Attribuez la ressource "1 TRG: Trade Group" à la "TASK 1" en créant un objet ResourceAssignment.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// Créez une définition d'attribut personnalisé avec une liste de recherche.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// Cette valeur peut être vue dans la vue "Resource usage" de MS Project.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### Voir aussi

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


