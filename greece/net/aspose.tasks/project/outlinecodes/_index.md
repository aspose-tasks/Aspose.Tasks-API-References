---
title: "Project.OutlineCodes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει το αντικείμενο OutlineCodeDefinitionCollection. Η συλλογή των ορισμών κωδικών περιγράμματος που σχετίζονται με ένα έργο"
type: docs
weight: 710
url: /el/net/aspose.tasks/project/outlinecodes/
---
## Project.OutlineCodes property

Λαμβάνει το αντικείμενο OutlineCodeDefinitionCollection. Η συλλογή των ορισμών κώδικα περιγράμματος που σχετίζονται με ένα έργο.

```csharp
public OutlineCodeDefinitionCollection OutlineCodes { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τους κωδικούς περιγράμματος.

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

    // Εμφάνιση μάσκας κωδικού περιγράμματος
    foreach (var outlineMask in ocd.Masks)
    {
        Console.WriteLine("Level of a mask = " + outlineMask.Level);
        Console.WriteLine("Mask = " + outlineMask);
    }

    // Εμφάνιση τιμών κωδικού περιγράμματος
    foreach (var outlineMask1 in ocd.Values)
    {
        Console.WriteLine("Description of outline value = " + outlineMask1.Description);
        Console.WriteLine("Value Id = " + outlineMask1.ValueId);
        Console.WriteLine("Value = " + outlineMask1.Value);
        Console.WriteLine("Type = " + outlineMask1.Type);
    }
}
```

### Δείτε επίσης

* class [OutlineCodeDefinitionCollection](../../outlinecodedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


