---
title: "Classe ExtendedAttribute"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ExtendedAttribute. Représente les attributs étendus"
type: docs
weight: 520
url: /fr/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Représente des attributs étendus.

```csharp
public class ExtendedAttribute
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Obtient la définition de l'attribut. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Obtient ou définit une valeur pour les attributs de type date (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | Obtient ou définit la valeur pour les attributs de type 'Duration'. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Obtient l'identifiant d'un champ. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | Obtient ou définit une valeur indiquant si un drapeau est défini pour un attribut de type 'Flag'. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Obtient si le calcul de la valeur de l'attribut étendu a entraîné une erreur. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Obtient ou définit une valeur pour les attributs de type numérique (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | Obtient ou définit une valeur pour les attributs de type 'Text'. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Obtient le guid d'une valeur de recherche. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Obtient une valeur indiquant si la valeur de cette instance `ExtendedAttribute` est en lecture seule. renvoie true si une formule ou un rollup est défini dans le [`ExtendedAttributeDefinition`](../extendedattributedefinition/) pour cet objet. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Renvoie une représentation courte sous forme de chaîne d'un attribut étendu. |

## Remarques

Actuellement, tous les types d'attributs étendus sont pris en charge lors de la lecture depuis MSP Xml 2003/2007 et mpp 2003. Pour MSP mpp 2007, la lecture de tous les attributs étendus est prise en charge sauf les durées et les drapeaux.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


