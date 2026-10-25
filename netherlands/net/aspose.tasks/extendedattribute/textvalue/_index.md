---
title: "ExtendedAttribute.TextValue"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttribute property. Haalt op of stelt een waarde in voor attributen met het type Text"
type: docs
weight: 80
url: /nl/net/aspose.tasks/extendedattribute/textvalue/
---
## ExtendedAttribute.TextValue property

Haalt op of stelt een waarde in voor attributen met het type 'Text'.

```csharp
public string TextValue { get; set; }
```

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| InvalidOperationException | Wordt gegooid als de [`AttributeDefinition`](../attributedefinition/) property niet is geïnitialiseerd of het huidige attribuut geen tekstattribuut is. |

## Voorbeelden

Toont hoe uitgebreide attributen toe te voegen die MS Project datum/tijd‑formules gebruiken.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// Stel de ProjDateDiff‑formule in en druk de waarde van het uitgebreide attribuut af.
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

// Stel de ProjDateSub‑formule in en druk de waarde van het uitgebreide attribuut af.
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// We kunnen de ProjDurConv‑formule instellen voor een duur‑gewaardeerd attribuut evenals voor een tekst‑gewaardeerd attribuut.
// Stel de ProjDurConv‑formule in voor een duur‑gewaardeerd uitgebreid attribuut en druk de waarde ervan af.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// Stel de ProjDurConv‑formule in voor een tekst‑gewaardeerd uitgebreid attribuut en druk de waarde ervan af.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Stel de Second‑formule in en druk de waarde van het uitgebreide attribuut af.
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Stel de Weekday‑formule in en druk de waarde van het uitgebreide attribuut af.
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### Zie ook

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


