---
title: "OutlineCode.ValueId"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "OutlineCode ιδιότητα. Λαμβάνει ή ορίζει το Id στη λίστα τιμών που σχετίζεται με τον ορισμό στη συλλογή κώδικα περιγράμματος"
type: docs
weight: 40
url: /el/net/aspose.tasks/outlinecode/valueid/
---
## OutlineCode.ValueId property

Λαμβάνει ή ορίζει το Id στη λίστα τιμών που σχετίζεται με τον ορισμό στη συλλογή κώδικα περιγράμματος.

```csharp
public int ValueId { get; set; }
```

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

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


