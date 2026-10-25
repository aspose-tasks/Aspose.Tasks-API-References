---
title: "Project.OutlineCodes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt het OutlineCodeDefinitionCollection-object op. De collectie van outline-code-definities die aan een project zijn gekoppeld."
type: docs
weight: 710
url: /nl/net/aspose.tasks/project/outlinecodes/
---
## Project.OutlineCodes property

Haalt OutlineCodeDefinitionCollection-object op. De collectie van outline code-definities die aan een project zijn gekoppeld.

```csharp
public OutlineCodeDefinitionCollection OutlineCodes { get; }
```

## Voorbeelden

Toont hoe outline-codes te lezen.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

foreach (var ocd in project.OutlineCodes)
{
    Console.WriteLine("Alias = " + ocd.Alias);
    Console.WriteLine(ocd.AllLevelsRequired ? "It contains property: must have all levels" : "It does not contain property: must have all levels");
    Console.WriteLine(ocd.Enterprise ? "It is an enterprise custom outline code." : "It is not an enterprise custom outline code.");
    Console.WriteLine("Reference to another custom field for which this outline code definition is an alias is = " + ocd.EnterpriseOutlineCodeAlias);
    Console.WriteLine("Field Id = " + ocd.FieldId);
    Console.WriteLine("Field Name = " + ocd.FieldName);
    Console.WriteLine("Phonetic Alias = " + ocd.PhoneticAlias);
    Console.WriteLine("Guid = " + ocd.Guid);

    // Toon outline-code-maskers
    foreach (var outlineMask in ocd.Masks)
    {
        Console.WriteLine("Level of a mask = " + outlineMask.Level);
        Console.WriteLine("Mask = " + outlineMask);
    }

    // Toon outline-code-waarden
    foreach (var outlineMask1 in ocd.Values)
    {
        Console.WriteLine("Description of outline value = " + outlineMask1.Description);
        Console.WriteLine("Value Id = " + outlineMask1.ValueId);
        Console.WriteLine("Value = " + outlineMask1.Value);
        Console.WriteLine("Type = " + outlineMask1.Type);
    }
}
```

### Zie ook

* class [OutlineCodeDefinitionCollection](../../outlinecodedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


