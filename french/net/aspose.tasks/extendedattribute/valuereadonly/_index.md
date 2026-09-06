---
title: "ExtendedAttribute.ValueReadOnly"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ExtendedAttribute. Obtient une valeur indiquant si la valeur de cette instance ExtendedAttribute est en lecture seule. renvoie true si une formule ou un rollup est défini dans le ExtendedAttributeDefinition pour cet objet"
type: docs
weight: 100
url: /fr/net/aspose.tasks/extendedattribute/valuereadonly/
---
## ExtendedAttribute.ValueReadOnly property

Obtient une valeur indiquant si la valeur de cette instance [`ExtendedAttribute`](../) est en lecture seule. renvoie true si une formule ou un rollup est défini dans le [`ExtendedAttributeDefinition`](../../extendedattributedefinition/) pour cet objet.

```csharp
public bool ValueReadOnly { get; }
```

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


