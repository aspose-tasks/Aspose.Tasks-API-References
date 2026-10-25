---
title: "Resource.TimephasedData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Resource. Λαμβάνει ή ορίζει ένα αντικείμενο της κλάσης TimephasedDataCollection για αυτό το αντικείμενο"
type: docs
weight: 740
url: /el/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

Αποκτά ή ορίζει μια παρουσία της κλάσης [`TimephasedDataCollection`](../../timephaseddatacollection/) για αυτό το αντικείμενο.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Παρατηρήσεις

Η ανάγνωση υποστηρίζεται μόνο για μορφή XML.

## Παραδείγματα

Δείχνει πώς να διαβάσετε δεδομένα χρονικής φάσης πόρων.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// επανάληψη πάνω στα δεδομένα χρονικής φάσης του πόρου 
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


