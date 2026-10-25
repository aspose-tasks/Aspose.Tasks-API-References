---
title: "OutlineCode.ValueGuid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "OutlineCode ιδιότητα. Λαμβάνει ή ορίζει το GUID της τιμής στη λίστα τιμών. Το ValueGuid ταιριάζει με το FieldGuid στη λίστα τιμών"
type: docs
weight: 30
url: /el/net/aspose.tasks/outlinecode/valueguid/
---
## OutlineCode.ValueGuid property

Λαμβάνει ή ορίζει το GUID της τιμής στη λίστα τιμών. Το ValueGuid ταιριάζει με το FieldGuid στη λίστα τιμών.

```csharp
public string ValueGuid { get; set; }
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


