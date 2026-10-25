---
title: "Enum OutlineValueType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OutlineValueType enum. Specificeert het type van een outline-waarde"
type: docs
weight: 1230
url: /nl/net/aspose.tasks/outlinevaluetype/
---
## OutlineValueType enumeration

Specificeert het type van een outline-waarde.

```csharp
public enum OutlineValueType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Null | `0` | Geeft Null outline-waarde type aan. |
| Date | `1` | Geeft datum outline-waarde type aan. |
| Duration | `2` | Geeft duur outline-waarde type aan. |
| Cost | `3` | Geeft kosten outline-waarde type aan. |
| Number | `4` | Geeft nummer outline-waarde type aan. |
| Flag | `5` | Geeft het type van de vlag-outlinewaarde aan. |
| Text | `6` | Geeft het type van de tekst-outlinewaarde aan. |
| FinishDate | `7` | Geeft het type van de Finish Date-outlinewaarde aan. |

## Voorbeelden

Toont hoe te werken met outline-waarden.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// maak een outline-waarde
var value = new OutlineValue();

// stel de werkelijke waarde in
value.Value = "Text value 1";

// stel de unieke Id van een outline-codewaarde binnen een project in
value.ValueId = 1;

// haal een GUID op die deze waarde identificeert onder andere in het gehele project
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// stel het outline-codetype in
value.Type = OutlineValueType.Text;

// stel de beschrijving van een outline-waarde in
value.Description = "Text value descr 1";

// stel een waarde in die aangeeft of de outline-waarde is samengevouwen of niet
value.IsCollapsed = false;

// controleer de Id van de bovenliggende waarde
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// maak een outline-waarde met duur
var value2 = new OutlineValue();

// stel de duurwaarde in
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// stel de unieke Id van een outline-codewaarde binnen een project in
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


