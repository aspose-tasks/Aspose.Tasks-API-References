---
title: "Task.TimephasedData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει ή ορίζει ένα αντικείμενο TimephasedDataCollection αυτού του task. Το μπλοκ δεδομένων χρονικής φάσης που σχετίζεται με ένα task"
type: docs
weight: 1220
url: /el/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

Λαμβάνει ή ορίζει ένα αντικείμενο TimephasedDataCollection αυτής της εργασίας. Το μπλοκ δεδομένων χρονικής φάσης που σχετίζεται με μια εργασία.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Παρατηρήσεις

Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

## Παραδείγματα

Δείχνει πώς να επαναλάβετε τα δεδομένα χρονικής φάσης του task.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


