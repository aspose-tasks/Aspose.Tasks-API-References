---
title: ExtendedAttributeDefinition.FieldId
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition property. Gets or sets corresponds to the project id of a custom field. Use string representation of a constant from ExtendedAttributeTask class to specify FieldId property
type: docs
weight: 130
url: /net/aspose.tasks/extendedattributedefinition/fieldid/
---
## ExtendedAttributeDefinition.FieldId property

Gets or sets corresponds to the project id of a custom field. Use string representation of a constant from [`ExtendedAttributeTask`](../../extendedattributetask/) class to specify `FieldId` property.

```csharp
public string FieldId { get; set; }
```

## Remarks

Preferable way to set `FieldId` property is to create [`ExtendedAttributeDefinition`](../) using one of the dedicated factory methods like [`CreateTaskDefinition`](../createtaskdefinition/) or [`CreateLookupTaskDefinition`](../createlookuptaskdefinition/).

## Examples

```csharp
customFieldDefinition.FieldId = Aspose.Tasks.ExtendedAttributeTask.Number10.ToString("D");
```

Shows how to read extended attribute definition common information.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// read extended attribute definition information
foreach (var definition in project.ExtendedAttributes)
{
    Console.WriteLine("Guid:" + definition.Guid);
    Console.WriteLine("Secondary Guid:" + definition.SecondaryGuid);
    Console.WriteLine("Secondary Pid:" + definition.SecondaryPid);
    Console.WriteLine("Alias:" + definition.Alias);
    Console.WriteLine("Phonetics Alias:" + definition.PhoneticsAlias);
    Console.WriteLine("Field Id:" + definition.FieldId);
    Console.WriteLine("Project Name:" + definition.ParentProject.Get(Prj.Name));

    Console.WriteLine("Append New Values:" + definition.AppendNewValues);
    Console.WriteLine("Auto RollDown:" + definition.AutoRollDown);
    Console.WriteLine("Calculation Type:" + definition.CalculationType);
    Console.WriteLine("Field Name" + definition.FieldName);
    Console.WriteLine("Is User Defined Custom Field:" + definition.UserDef);
    Console.WriteLine("Rollup Type:" + definition.RollupType);

    if (definition.CalculationType == CalculationType.Lookup)
    {
        Console.WriteLine("  Next properties are used only for lookups:");
        Console.WriteLine("  Default Guid:" + definition.DefaultGuid);
        Console.WriteLine("  Element Type:" + definition.ElementType);
        Console.WriteLine("  Lookup Uid:" + definition.LookupUid);
        Console.WriteLine("  Restrict Values:" + definition.RestrictValues);
        Console.WriteLine("  Max Multi Values:" + definition.MaxMultiValues);
        Console.WriteLine("  Valuelist Sort Order:" + definition.ValuelistSortOrder);
        Console.WriteLine("  Default Value:" + definition.Default);
        Console.WriteLine("  Print values from value list:");
        foreach (var value in definition.ValueList)
        {
            Console.WriteLine("    Description: " + value.Description);
            Console.WriteLine("    Value: " + value.Val);
        }
    }

    Console.WriteLine();
}
```

### See Also

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


