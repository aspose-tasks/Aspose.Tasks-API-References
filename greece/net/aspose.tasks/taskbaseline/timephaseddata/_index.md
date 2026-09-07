---
title: "TaskBaseline.TimephasedData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskBaseline property. Λαμβάνει ή ορίζει μια παρουσία της TimephasedDataCollection για αυτό το αντικείμενο. Τα χρονομετρικά δεδομένα που σχετίζονται με τη βάση εργασίας"
type: docs
weight: 80
url: /el/net/aspose.tasks/taskbaseline/timephaseddata/
---
## TaskBaseline.TimephasedData property

Λαμβάνει ή ορίζει μια παρουσία της TimephasedDataCollection για αυτό το αντικείμενο. Τα δεδομένα φάσης χρόνου που σχετίζονται με τη βάση αναφοράς της εργασίας.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αποκτήσετε πρόσβαση σε πληροφορίες βάσης αναφοράς.

```csharp
var project = new Project();

// Δημιουργία TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Εμφάνιση διάρκειας βάσης αναφοράς εργασίας
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// τιμή που υποδεικνύει εάν πρόκειται για ενδιάμεση βάση αναφοράς
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// εκτύπωση δεδομένων φάσης χρόνου της βάσης αναφοράς εργασίας
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### Δείτε επίσης

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


