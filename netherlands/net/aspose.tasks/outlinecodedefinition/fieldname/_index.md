---
title: "OutlineCodeDefinition.FieldName"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OutlineCodeDefinition property. Haalt op of stelt de naam van een aangepaste outlinecode in"
type: docs
weight: 70
url: /nl/net/aspose.tasks/outlinecodedefinition/fieldname/
---
## OutlineCodeDefinition.FieldName property

Haalt op of stelt de naam in van een aangepaste outline code.

```csharp
public string FieldName { get; set; }
```

## Voorbeelden

Toont hoe te werken met outline-code-definities.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// maak een nieuwe outline-code-definitie
var outline = new OutlineCodeDefinition();

// stel het veldnummer van een outline-code in
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// stel de naam van een aangepaste outline-code in
outline.FieldName = "Outline Code1";

// stel de Guid van een outline-code in
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// stel een waarde in die aangeeft of de in dit outline-codeveld gespecificeerde waarden bladwaarden moeten zijn
outline.LeafOnly = false;

// stel de alias van een aangepaste outline-code in
outline.Alias = "My Outline Code";

// stel de fonetische uitspraak van de alias van de aangepaste outline-code in
outline.PhoneticAlias = "Outline Code";

// stel een waarde in die aangeeft of de nieuwe codes alle niveaus moeten hebben. Niet beschikbaar voor Enterprise Codes.
outline.AllLevelsRequired = true;

// stel een waarde in die aangeeft of een aangepaste outline-code een enterprise aangepaste outline-code is
outline.Enterprise = false;

// stel een referentie in naar een ander aangepast veld waarvoor deze outline-code-definitie een alias is
outline.EnterpriseOutlineCodeAlias = 0;

// voeg een outline-masker toe
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// stel een waarde in die aangeeft of de gespecificeerde waarden uit de waardentabel moeten komen
outline.OnlyTableValuesAllowed = false;

// stel een waarde in die aangeeft of de aangepaste outline-code kan worden gebruikt
// door de Resource Substitution Wizard in Microsoft Project
outline.ResourceSubstitutionEnabled = false;

// stel een waarde in die aangeeft of de inspringingen van deze outline-code moeten worden weergegeven.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Zie ook

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


