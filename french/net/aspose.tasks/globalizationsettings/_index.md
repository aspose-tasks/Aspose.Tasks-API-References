---
title: "Classe GlobalizationSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.GlobalizationSettings. Représente les paramètres de mondialisation du projet"
type: docs
weight: 720
url: /fr/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Représente les paramètres de mondialisation du projet.

```csharp
public class GlobalizationSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Obtient une chaîne pour le littéral booléen 'false' utilisé dans une formule. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Obtient le littéral "NA" (valeur vide) utilisé dans une formule pour un champ de date. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Obtient une chaîne pour le littéral booléen 'true' utilisé dans une formule. |

## Remarques

La façon recommandée est d'utiliser des littéraux ou des formats indépendants de la culture dans tout le projet. Cependant, si un projet utilise des littéraux spécifiques à une culture, cette classe peut être utilisée pour aider le moteur de calcul de formules à analyser ces littéraux.

## Exemples

Montre comment définir les paramètres linguistiques spécifiques du projet.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Créer un attribut étendu
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


