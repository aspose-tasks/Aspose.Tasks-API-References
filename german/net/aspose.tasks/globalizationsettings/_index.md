---
title: "Klasse GlobalizationSettings"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.GlobalizationSettings Klasse. Stellt die Globalisierungseinstellungen des Projekts dar"
type: docs
weight: 720
url: /de/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Stellt die Globalisierungseinstellungen des Projekts dar.

```csharp
public class GlobalizationSettings
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Gibt einen String für das boolesche 'false'-Literal zurück, das in einer Formel verwendet wird. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Gibt das Literal "NA" (leerer Wert) zurück, das in einer Formel für ein Datumsfeld verwendet wird. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Gibt einen String für das boolesche 'true'-Literal zurück, das in einer Formel verwendet wird. |

## Hinweise

Empfohlen wird, kulturunabhängige Literale oder Formate im gesamten Projekt zu verwenden. Wenn ein Projekt jedoch kulturspezifische Literale verwendet, kann diese Klasse eingesetzt werden, um der Formel‑Berechnungs‑Engine beim Parsen dieser Literale zu helfen.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


