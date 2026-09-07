---
title: "ExtendedAttributeDefinition.ValueList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttributeDefinition. Λαμβάνει το ListValue ValueList"
type: docs
weight: 280
url: /el/net/aspose.tasks/extendedattributedefinition/valuelist/
---
## ExtendedAttributeDefinition.ValueList property

Λαμβάνει τη λίστα List&lt;Value&gt; ValueList.

```csharp
public List<Value> ValueList { get; }
```

## Παρατηρήσεις

Όταν οι τιμές των εκτεταμένων ιδιοτήτων καθορίζονται ως ιδιότητες των στοιχείων στο σχήμα, μπορούν είτε να καθοριστούν με τιμές είτε με αναφορές στις τιμές που περιέχονται σε αυτή τη λίστα. Οι εφαρμογές μπορούν να υποθέτουν τη σειρά της λίστας βάσει της σειράς που καθορίζεται εδώ. Επί του παρόντος υποστηρίζεται για τις μορφές MSP 2003/2007 Xml και MSP 2003 mpp. Μην αλλάζετε αυτή τη λίστα απευθείας. Χρησιμοποιήστε τις μεθόδους ExtendedAttributeDefinition.AddLookupValue/RemoveLookupValue αντί αυτού.

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις κοινές πληροφορίες του ορισμού εκτεταμένου χαρακτηριστικού.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

// διαβάστε πληροφορίες ορισμού εκτεταμένου χαρακτηριστικού
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

### Δείτε επίσης

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


