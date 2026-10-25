---
title: "ExtendedAttribute.NumericValue"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ExtendedAttribute. Obtient ou définit une valeur pour les attributs de types numériques Cost Number"
type: docs
weight: 70
url: /fr/net/aspose.tasks/extendedattribute/numericvalue/
---
## ExtendedAttribute.NumericValue property

Obtient ou définit une valeur pour les attributs de type numérique (Cost, Number).

```csharp
public decimal NumericValue { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Lancée si la propriété [`AttributeDefinition`](../attributedefinition/) n'est pas initialisée ou si le type de champ personnalisé de la propriété [`AttributeDefinition`](../attributedefinition/) n'est pas 'Cost' ou 'Number'. |

## Exemples

Montre comment ajouter un champ personnalisé dont la valeur est calculée à l'aide d'une formule spécifiée par l'utilisateur.

```csharp
var project = new Project();

// créer une nouvelle définition d'attribut étendu de tâche
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Ajoutez une formule à l'attribut.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Créer un attribut étendu
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// Nous définissons la Formule pour l'attribut étendu, de sorte qu'il soit en lecture seule (la valeur est calculée à l'aide de la formule).
// La sortie est "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// Vous pouvez essayer de définir la valeur d'un champ en lecture seule, mais cela n'aura aucun effet.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### Voir aussi

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


