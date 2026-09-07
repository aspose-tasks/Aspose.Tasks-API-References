---
title: "Κλάση EntityFieldAttribute"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Attributes.EntityFieldAttribute class. Αντιπροσωπεύει ένα χαρακτηριστικό για ιδιότητες οντοτήτων"
type: docs
weight: 70
url: /el/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Αντιπροσωπεύει ένα χαρακτηριστικό για ιδιότητες οντοτήτων.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Παρατηρήσεις

Χαρακτηριστικό που χρησιμοποιείται μόνο για ιδιότητες οντοτήτων [`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) και [`ResourceAssignment`](../../aspose.tasks/resourceassignment/), και απλοποιεί την απαρίθμησή του.

## Παραδείγματα

Πώς να απαριθμήσετε ιδιότητες χρησιμοποιώντας το χαρακτηριστικό **EntityField**:

```csharp
[C#]
var project = new Project("sample.mpp");
foreach (var task in project.SelectAllChildTasks())
{
    Console.WriteLine("Task:");
    foreach (var propInfo in typeof(Task).GetProperties().Where(propInfo => propInfo.GetCustomAttribute{Attributes.EntityFieldAttribute}() != null))
    {
        Console.WriteLine(string.Format("{0}: {1}", propInfo.Name, propInfo.GetValue(task)));
    }
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


