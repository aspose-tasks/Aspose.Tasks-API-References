---
title: "Project.GlobalizationSettings"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Project-Eigenschaft. Ruft die globalen, sprachspezifischen Einstellungen des Projekts ab oder legt sie fest."
type: docs
weight: 460
url: /de/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

Ruft die Globalisierungs‑(sprachspezifischen) Einstellungen des Projekts ab oder legt sie fest.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## Hinweise

Die empfohlene Vorgehensweise besteht darin, kulturunabhängige Literale oder Formate im gesamten Projekt zu verwenden. Sollte ein Projekt jedoch kulturabhängige Literale verwenden, kann diese Klasse verwendet werden, um der Berechnungs‑Engine beim Parsen dieser Literale zu helfen.

## Beispiele

Zeigt, wie die sprachspezifischen Einstellungen des Projekts festgelegt werden.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Erstelle erweitertes Attribut
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### Siehe auch

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


