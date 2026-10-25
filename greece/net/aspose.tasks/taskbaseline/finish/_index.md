---
title: "TaskBaseline.Finish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα TaskBaseline. Λαμβάνει ή ορίζει την προγραμματισμένη ημερομηνία λήξης της εργασίας όταν αποθηκεύτηκε το baseline"
type: docs
weight: 40
url: /el/net/aspose.tasks/taskbaseline/finish/
---
## TaskBaseline.Finish property

Λαμβάνει ή ορίζει την προγραμματισμένη ημερομηνία λήξης της εργασίας όταν αποθηκεύτηκε η βάση αναφοράς.

```csharp
public DateTime Finish { get; set; }
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

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


