---
title: "Project.GlobalizationSettings"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient ou définit les paramètres de mondialisation spécifiques à la langue du projet"
type: docs
weight: 460
url: /fr/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

Obtient ou définit les paramètres de mondialisation (spécifiques à la langue) du projet.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## Remarques

La méthode recommandée consiste à utiliser des littéraux ou des formats indépendants de la culture dans tout le projet. Cependant, si un projet utilise des littéraux spécifiques à une culture, cette classe peut être utilisée pour aider le moteur de calcul à analyser ces littéraux.

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


