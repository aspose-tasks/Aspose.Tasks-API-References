---
title: "ExtendedAttribute.DurationValue"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ExtendedAttribute. Obtient ou définit la valeur pour les attributs de type Durée"
type: docs
weight: 30
url: /fr/net/aspose.tasks/extendedattribute/durationvalue/
---
## ExtendedAttribute.DurationValue property

Obtient ou définit la valeur pour les attributs de type 'Duration'.

```csharp
public Duration DurationValue { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Lancée si la propriété [`AttributeDefinition`](../attributedefinition/) n'est pas initialisée ou si le type de champ personnalisé de la propriété [`AttributeDefinition`](../attributedefinition/) n'est pas une instance de [`Duration`](../../duration/). |

## Exemples

Montre comment ajouter des attributs étendus qui utilisent les formules de date/heure de MS Project.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// Définissez la formule ProjDateDiff et affichez la valeur de l'attribut étendu
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// Définissez la formule ProjDateSub et affichez la valeur de l'attribut étendu
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// Nous pouvons définir la formule ProjDurConv pour un attribut de type durée ainsi que pour un attribut de type texte.
// Définissez la formule ProjDurConv sur l'attribut étendu de type durée et affichez sa valeur.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// Définissez la formule ProjDurConv sur l'attribut étendu de type texte et affichez sa valeur.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Définissez la formule Second et affichez la valeur de l'attribut étendu
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Définissez la formule Weekday et affichez la valeur de l'attribut étendu
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### Voir aussi

* struct [Duration](../../duration/)
* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


