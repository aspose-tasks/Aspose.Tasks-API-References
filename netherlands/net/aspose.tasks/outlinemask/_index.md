---
title: "Klasse OutlineMask"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OutlineMask klasse. Geeft vier elementen van een masker weer die een outline-codeformaat definiëren."
type: docs
weight: 1190
url: /nl/net/aspose.tasks/outlinemask/
---
## OutlineMask class

Stelt vier elementen van een masker voor die een outline‑code‑formaat definieert.

```csharp
public class OutlineMask
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [OutlineMask](outlinemask/)() | Initialiseert een nieuw exemplaar van de `OutlineMask` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | Haalt de maximale lengte (in tekens) van de outline-codewaarden op of stelt deze in. 0 als de lengte niet is gedefinieerd. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | Haalt het niveau van een masker op of stelt dit in. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | Haalt de scheidingsteken van codewaarden op of stelt deze in. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | Haalt het type van een masker op of stelt dit in. |

## Voorbeelden

Toont hoe te werken met outline-masks.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// stel het type van een masker in
mask.Type = MaskType.Characters;

// stel de scheidingsteken van codewaarden in
mask.Separator = "/";

// stel het niveau van een masker in
mask.Level = 1;

// stel de maximale lengte (in tekens) van de outline-codewaarden in. 0 als de lengte niet is gedefinieerd.
mask.Length = 2;

// voeg het masker toe aan de definitie
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


