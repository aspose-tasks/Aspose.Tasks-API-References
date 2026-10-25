---
title: "ExtendedAttributeDefinition.FieldId"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ExtendedAttributeDefinition. Ottiene o imposta il valore corrispondente all'ID progetto di un campo personalizzato. Usa la rappresentazione stringa di una costante della classe ExtendedAttributeTask per specificare la proprietà FieldId"
type: docs
weight: 130
url: /it/net/aspose.tasks/extendedattributedefinition/fieldid/
---
## ExtendedAttributeDefinition.FieldId property

Ottiene o imposta il valore corrispondente all'ID progetto di un campo personalizzato. Usa la rappresentazione stringa di una costante della classe [`ExtendedAttributeTask`](../../extendedattributetask/) per specificare la proprietà `FieldId`.

```csharp
public string FieldId { get; set; }
```

## Osservazioni

Il modo consigliato per impostare la proprietà `FieldId` è creare [`ExtendedAttributeDefinition`](../) utilizzando uno dei metodi di fabbrica dedicati come [`CreateTaskDefinition`](../createtaskdefinition/) o [`CreateLookupTaskDefinition`](../createlookuptaskdefinition/).

## Esempi

```csharp
customFieldDefinition.FieldId = Aspose.Tasks.ExtendedAttributeTask.Number10.ToString("D");
```

Mostra come leggere le informazioni comuni della definizione di attributo esteso.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// leggi le informazioni della definizione di attributo esteso
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

### Vedi anche

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


