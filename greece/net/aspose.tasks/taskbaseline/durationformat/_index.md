---
title: "DurationFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Λαμβάνει ή ορίζει τη μορφή για την έκφραση της διάρκειας της βάσης εργασίας."
type: docs
weight: 30
url: /el/net/aspose.tasks/taskbaseline/durationformat/
---
## TaskBaseline.DurationFormat property

Λαμβάνει ή ορίζει τη μορφή για την έκφραση της διάρκειας της βάσης εργασίας.

```csharp
public TimeUnitType DurationFormat { get; set; }
```

### Παραδείγματα

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
Console.WriteLine("Baseline duration format: {0}", baseline.DurationFormat);
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

* enum [TimeUnitType](../../timeunittype)
* class [TaskBaseline](../../taskbaseline)
* namespace [Aspose.Tasks](../../taskbaseline)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
