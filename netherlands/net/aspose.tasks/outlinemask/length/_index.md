---
title: "OutlineMask.Length"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OutlineMask-eigenschap. Haalt de maximale lengte in tekens van de outline-codewaarden op of stelt deze in. 0 als de lengte niet is gedefinieerd"
type: docs
weight: 20
url: /nl/net/aspose.tasks/outlinemask/length/
---
## OutlineMask.Length property

Haalt de maximale lengte (in tekens) van de outline-codewaarden op of stelt deze in. 0 als de lengte niet is gedefinieerd.

```csharp
public int Length { get; set; }
```

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

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


