---
title: OutlineCodeDefinition.Masks
second_title: Aspose.Tasks for .NET API Reference
description: OutlineCodeDefinition property. Gets the OutlineMaskCollection object. The table of entries that define the outline code mask. Readonly OutlineMaskCollection instance
type: docs
weight: 100
url: /net/aspose.tasks/outlinecodedefinition/masks/
---
## OutlineCodeDefinition.Masks property

Gets the OutlineMaskCollection object. The table of entries that define the outline code mask. Read-only [`OutlineMaskCollection`](../../outlinemaskcollection/) instance.

```csharp
public OutlineMaskCollection Masks { get; }
```

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

* class [OutlineMaskCollection](../../outlinemaskcollection/)
* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


