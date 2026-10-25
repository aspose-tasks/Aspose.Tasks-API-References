---
title: "Class GlobalizationSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.GlobalizationSettings class. Rappresenta le impostazioni di globalizzazione del progetto"
type: docs
weight: 720
url: /it/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Rappresenta le impostazioni di globalizzazione del progetto.

```csharp
public class GlobalizationSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Ottiene una stringa per il letterale booleano 'false' usato in una formula. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Ottiene il letterale "NA" (valore vuoto) usato in una formula per un campo data. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Ottiene una stringa per il letterale booleano 'true' utilizzato in una formula. |

## Osservazioni

Il modo consigliato è utilizzare letterali o formati indipendenti dalla cultura in tutto il progetto. Tuttavia, se un progetto utilizza letterali specifici per la cultura, questa classe può essere usata per aiutare il motore di calcolo delle formule a interpretare tali letterali.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


