---
title: "ExtendedAttributeDefinition.ElementType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition eigenschap. Haalt een waarde op of stelt deze in dat het uitgebreide attribuut is gekoppeld aan een taak, een resource of een toewijzing"
type: docs
weight: 120
url: /nl/net/aspose.tasks/extendedattributedefinition/elementtype/
---
## ExtendedAttributeDefinition.ElementType property

Haalt op of stelt in of het uitgebreide attribuut is gekoppeld aan een taak, een resource of een toewijzing.

```csharp
public ElementType ElementType { get; set; }
```

## Voorbeelden

Toont hoe je algemene informatie van een uitgebreide attribuutdefinitie kunt lezen.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// lees informatie van uitgebreide attribuutdefinitie
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

### Zie ook

* enum [ElementType](../../elementtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


