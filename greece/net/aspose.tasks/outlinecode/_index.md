---
title: "Κλάση OutlineCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.OutlineCode class. Αντιπροσωπεύει μια τιμή ενός κώδικα περιγράμματος"
type: docs
weight: 1150
url: /el/net/aspose.tasks/outlinecode/
---
## OutlineCode class

Αντιπροσωπεύει μια τιμή ενός κώδικα περίγραμμα.

```csharp
public class OutlineCode
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `OutlineCode`. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | Αρχικοποιεί μια νέα παρουσία της κλάσης `OutlineCode` χρησιμοποιώντας τον καθορισμένο Outline Code και μία από τις τιμές του. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | Λαμβάνει ή ορίζει την αριθμητική τιμή του προσαρμοσμένου πεδίου Id του έργου. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | Λαμβάνει ή ορίζει το GUID της τιμής στη λίστα τιμών. Το ValueGuid ταιριάζει με το FieldGuid στη λίστα τιμών. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | Λαμβάνει ή ορίζει το Id στη λίστα τιμών που σχετίζεται με τον ορισμό στη συλλογή κώδικα περιγράμματος. |

## Παρατηρήσεις

Απαιτούνται δύο στοιχεία δεδομένων - ένας δείκτης στον πίνακα κώδικα περιγράμματος που καθορίζεται από το FieldId, και η τιμή που καθορίζεται είτε από το ValueId είτε από το ValueGuid δείκτη στη λίστα τιμών.

## Παραδείγματα

Δείχνει πώς να διαβάσετε τους κώδικες περιγράμματος του task.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// διαβάστε κώδικες περιγράμματος
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


