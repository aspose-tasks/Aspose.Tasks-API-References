---
title: Class OutlineCodeDefinition
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.OutlineCodeDefinition class. Represents an outline code definition
type: docs
weight: 1160
url: /net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

Represents an outline code definition.

```csharp
public sealed class OutlineCodeDefinition
```

## Constructors

| Name | Description |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | Initializes a new instance of the `OutlineCodeDefinition` class. |

## Properties

| Name | Description |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | Gets or sets the alias of a custom outline code. |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | Gets or sets a value indicating whether the new codes must have all levels. Not available for Enterprise Codes. |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | Gets or sets a value indicating whether a custom outline code is an enterprise custom outline code. |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | Gets or sets a reference to another custom field for which this outline code definition is an alias. |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | Gets or sets the field number of an outline code. |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | Gets or sets the name of a custom outline code. |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | Gets or sets the Guid of an outline code. |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | Gets or sets a value indicating whether the values specified in this outline code field must be leaf values. |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | Gets the OutlineMaskCollection object. The table of entries that define the outline code mask. Read-only [`OutlineMaskCollection`](../outlinemaskcollection/) instance. |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | Gets or sets a value indicating whether the values specified must come from values table. |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | Gets or sets the phonetic pronunciation of the alias of the custom outline code. |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | Gets or sets a value indicating whether the custom outline code can be used by the Resource Substitution Wizard in Microsoft Project. |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | Gets or sets a value indicating whether the indents of this outline code must be shown. |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | Gets OutlineValueCollection object. The values of the table associated with this outline code. |

## Examples

Shows how to work with outline code definitions.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// create a new outline code definition
var outline = new OutlineCodeDefinition();

// set the field number of an outline code
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// set the name of a custom outline code
outline.FieldName = "Outline Code1";

// set the Guid of an outline code
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// set a value indicating whether the values specified in this outline code field must be leaf values
outline.LeafOnly = false;

// set the alias of a custom outline code
outline.Alias = "My Outline Code";

// set the phonetic pronunciation of the alias of the custom outline code
outline.PhoneticAlias = "Outline Code";

// set a value indicating whether the new codes must have all levels. Not available for Enterprise Codes.
outline.AllLevelsRequired = true;

// set a value indicating whether a custom outline code is an enterprise custom outline code
outline.Enterprise = false;

// set a reference to another custom field for which this outline code definition is an alias
outline.EnterpriseOutlineCodeAlias = 0;

// add an outline mask
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// set a value indicating whether the values specified must come from values table
outline.OnlyTableValuesAllowed = false;

// set a value indicating whether the custom outline code can be used
// by the Resource Substitution Wizard in Microsoft Project
outline.ResourceSubstitutionEnabled = false;

// set a value indicating whether the indents of this outline code must be shown.
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

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


