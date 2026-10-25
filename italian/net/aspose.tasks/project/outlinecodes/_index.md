---
title: "Project.OutlineCodes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene l'oggetto OutlineCodeDefinitionCollection. La collezione delle definizioni dei codici di struttura associati a un progetto"
type: docs
weight: 710
url: /it/net/aspose.tasks/project/outlinecodes/
---
## Project.OutlineCodes property

Ottiene l'oggetto OutlineCodeDefinitionCollection. La collezione delle definizioni di codice di struttura associate a un progetto.

```csharp
public OutlineCodeDefinitionCollection OutlineCodes { get; }
```

## Esempi

Mostra come leggere i codici di struttura.

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

    // Visualizza le maschere dei codici di struttura
    foreach (var outlineMask in ocd.Masks)
    {
        Console.WriteLine("Level of a mask = " + outlineMask.Level);
        Console.WriteLine("Mask = " + outlineMask);
    }

    // Visualizza i valori dei codici di struttura
    foreach (var outlineMask1 in ocd.Values)
    {
        Console.WriteLine("Description of outline value = " + outlineMask1.Description);
        Console.WriteLine("Value Id = " + outlineMask1.ValueId);
        Console.WriteLine("Value = " + outlineMask1.Value);
        Console.WriteLine("Type = " + outlineMask1.Type);
    }
}
```

### Vedi anche

* class [OutlineCodeDefinitionCollection](../../outlinecodedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


