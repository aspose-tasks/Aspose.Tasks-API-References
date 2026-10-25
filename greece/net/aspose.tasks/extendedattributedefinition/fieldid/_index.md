---
title: "ExtendedAttributeDefinition.FieldId"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttributeDefinition. Λαμβάνει ή ορίζει που αντιστοιχεί στο αναγνωριστικό έργου ενός προσαρμοσμένου πεδίου. Χρησιμοποιήστε την αναπαράσταση συμβολοσειράς μιας σταθεράς από την κλάση ExtendedAttributeTask για να καθορίσετε την ιδιότητα FieldId"
type: docs
weight: 130
url: /el/net/aspose.tasks/extendedattributedefinition/fieldid/
---
## ExtendedAttributeDefinition.FieldId property

Λαμβάνει ή ορίζει που αντιστοιχεί στο αναγνωριστικό έργου ενός προσαρμοσμένου πεδίου. Χρησιμοποιήστε την αναπαράσταση συμβολοσειράς μιας σταθεράς από την κλάση [`ExtendedAttributeTask`](../../extendedattributetask/) για να καθορίσετε την ιδιότητα `FieldId`.

```csharp
public string FieldId { get; set; }
```

## Παρατηρήσεις

Ο προτιμώμενος τρόπος για να ορίσετε την ιδιότητα `FieldId` είναι να δημιουργήσετε το [`ExtendedAttributeDefinition`](../) χρησιμοποιώντας μία από τις ειδικές μεθόδους κατασκευής όπως το [`CreateTaskDefinition`](../createtaskdefinition/) ή το [`CreateLookupTaskDefinition`](../createlookuptaskdefinition/).

## Παραδείγματα

```csharp
customFieldDefinition.FieldId = Aspose.Tasks.ExtendedAttributeTask.Number10.ToString("D");
```

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

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


