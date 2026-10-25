---
title: "ExtendedAttributeDefinition.AddLookupValue"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ExtendedAttributeDefinition. Ajoute une valeur à la liste de recherche interne. C'est la façon préférée de manipuler la ValueList"
type: docs
weight: 300
url: /fr/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Ajoute une valeur à la liste de recherche interne. C'est la façon préférée de manipuler le [`ValueList`](../valuelist/).

```csharp
public void AddLookupValue(Value value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| value | Valeur | Valeur à ajouter à la recherche. |

## Remarques

Cette méthode fonctionne uniquement pour les instances de [`ExtendedAttributeDefinition`](../) qui ont [`CalculationType`](../calculationtype/) égal à Lookup.

## Exemples

Utilisez ce code pour ajouter une nouvelle Valeur à la liste de recherche :

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

Montre comment ajouter des attributs étendus avec des listes de recherche pour les affectations.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Attribuez la ressource "1 TRG: Trade Group" à la "TASK 1" en créant un objet ResourceAssignment.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Créez une définition d'attribut personnalisé avec une liste de recherche.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Cette valeur peut être vue dans la vue "Resource usage" de MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Créez une définition d'attribut personnalisé avec une liste de recherche.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Cette valeur peut être vue dans la vue "Task usage" de MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// Des valeurs incorrectes peuvent être supprimées ultérieurement.
taskCostAttr.RemoveLookupValue(taskWrongValue);

// Travail avec le projet...
```

### Voir aussi

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


