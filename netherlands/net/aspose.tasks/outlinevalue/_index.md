---
title: "Class OutlineValue"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OutlineValue class. Vertegenwoordigt een outline‑waarde"
type: docs
weight: 1210
url: /nl/net/aspose.tasks/outlinevalue/
---
## OutlineValue class

Stelt een outline‑waarde voor.

```csharp
public class OutlineValue
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [OutlineValue](outlinevalue/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Description](../../aspose.tasks/outlinevalue/description/) { get; set; } | Haalt de beschrijving van een outline-waarde op of stelt deze in. |
| [DurationValue](../../aspose.tasks/outlinevalue/durationvalue/) { get; set; } | Haalt de duur op of stelt deze in als Type Duration is. |
| [IsCollapsed](../../aspose.tasks/outlinevalue/iscollapsed/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of de outline-waarde is samengevouwen of niet. |
| [ParentValueId](../../aspose.tasks/outlinevalue/parentvalueid/) { get; set; } | Haalt de Id op of stelt deze in van een bovenliggend knooppunt van een outline-code. |
| [Type](../../aspose.tasks/outlinevalue/type/) { get; set; } | Haalt het type van de outline-code op of stelt dit in. |
| [Value](../../aspose.tasks/outlinevalue/value/) { get; set; } | Haalt de werkelijke waarde op of stelt deze in. |
| [ValueGuid](../../aspose.tasks/outlinevalue/valueguid/) { get; } | Haalt een GUID op die deze waarde identificeert tussen andere in het gehele project. |
| [ValueId](../../aspose.tasks/outlinevalue/valueid/) { get; set; } | Haalt de unieke Id op of stelt deze in van een outline-codewaarde binnen een project. |

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


