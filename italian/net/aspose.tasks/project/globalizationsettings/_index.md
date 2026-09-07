---
title: "Project.GlobalizationSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà del progetto. Ottiene o imposta le impostazioni specifiche della lingua per la globalizzazione del progetto"
type: docs
weight: 460
url: /it/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

Ottiene o imposta le impostazioni di globalizzazione (specifiche della lingua) del progetto.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## Osservazioni

Il modo consigliato è utilizzare letterali o formati indipendenti dalla cultura in tutto il progetto. Tuttavia, se un progetto utilizza letterali specifici della cultura, questa classe può essere usata per aiutare il motore di calcolo a interpretare tali letterali.

## Esempi

Mostra come impostare le impostazioni specifiche della lingua del progetto.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Crea attributo esteso
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### Vedi anche

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


