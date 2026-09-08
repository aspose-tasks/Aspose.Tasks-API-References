---
title: "Klasse OutlineCodeDefinition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OutlineCodeDefinition klasse. Vertegenwoordigt een outline code definitie."
type: docs
weight: 1170
url: /nl/net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

Stelt een definitie van een outline‑code voor.

```csharp
public sealed class OutlineCodeDefinition
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | Initialiseert een nieuw exemplaar van de `OutlineCodeDefinition` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | Haalt op of stelt de alias in van een aangepaste outline code. |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de nieuwe codes alle niveaus moeten hebben. Niet beschikbaar voor Enterprise-codes. |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een aangepaste outline code een enterprise aangepaste outline code is. |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | Haalt op of stelt een referentie in naar een ander aangepast veld waarvoor deze outline code definitie een alias is. |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | Haalt op of stelt het veldnummer in van een outline code. |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | Haalt op of stelt de naam in van een aangepaste outline code. |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | Haalt op of stelt de Guid in van een outline code. |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de waarden gespecificeerd in dit outline code veld bladwaarden moeten zijn. |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | Haalt het OutlineMaskCollection-object op. De tabel met items die de outline code mask definiëren. Alleen-lezen [`OutlineMaskCollection`](../outlinemaskcollection/) instantie. |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de gespecificeerde waarden uit de waardentabel moeten komen. |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | Haalt op of stelt de fonetische uitspraak in van de alias van de aangepaste outline code. |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de aangepaste outline code kan worden gebruikt door de Resource Substitution Wizard in Microsoft Project. |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de inspringingen van deze outline code moeten worden weergegeven. |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | Haalt OutlineValueCollection-object op. De waarden van de tabel die aan deze outline-code zijn gekoppeld. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


