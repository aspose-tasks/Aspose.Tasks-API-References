---
title: "Κλάση TimephasedData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.TimephasedData. Αντιπροσωπεύει δεδομένα χρονικής φάσης"
type: docs
weight: 2590
url: /el/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

Αντιπροσωπεύει δεδομένα χρονικής φάσης.

```csharp
public class TimephasedData
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [TimephasedData](timephaseddata/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `TimephasedData`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία λήξης μιας περιόδου δεδομένων χρονικής φάσης. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία έναρξης μιας περιόδου δεδομένων χρονικής φάσης. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο ενός δεδομένου χρονικής φάσης. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό ενός δεδομένου χρονικής φάσης |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | Λαμβάνει ή ορίζει τη μονάδα χρόνου μιας περιόδου δεδομένων χρονικής φάσης. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | Λαμβάνει ή ορίζει την τιμή ανά μονάδα χρόνου για μια περίοδο δεδομένων χρονικής φάσης. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | Λαμβάνει την παρουσία Double που αντιπροσωπεύει τη συμβολοσειρά τιμής αυτού του αντικειμένου. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | Λαμβάνει την παρουσία TimeSpan που αντιπροσωπεύει τη συμβολοσειρά τιμής αυτού του αντικειμένου. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | Λαμβάνει την παρουσία Double που αντιπροσωπεύει τη συμβολοσειρά τιμής αυτού του αντικειμένου για δεδομένα χρονικής φάσης βάσει μονάδας. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης `TimephasedData` για δεδομένα χρονικής φάσης βάσει κόστους. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης `TimephasedData` για δεδομένα χρονικής φάσης βάσει κόστους. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης `TimephasedData` για δεδομένα χρονικής φάσης βάσει μονάδας μιας ανάθεσης υλικού πόρου |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | Δημιουργεί και αρχικοποιεί ένα νέο αντικείμενο της κλάσης `TimephasedData` για δεδομένα χρονομερισμένα με βάση την εργασία. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με προσαρμοσμένα δεδομένα χρονικής φάσης.

```csharp
var project = new Project(DataDir + "Project1.mpp") { CalculationMode = CalculationMode.None };

var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2018, 1, 1, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var workAssignment = project.ResourceAssignments.Add(task, workResource);
workAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);
var costAssignment = project.ResourceAssignments.Add(task, costResource);
costAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);

// ας προσθέσουμε προσαρμοσμένα χρονικά tds
workAssignment.TimephasedData.Clear();

// προσθέστε εργάσιμες ημέρες
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// προσθέστε Σαββατοκύριακο
var td2 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    TimeSpan.Zero,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

workAssignment.TimephasedData.Add(td1);
workAssignment.TimephasedData.Add(td2);

costAssignment.TimephasedData.Clear();

// προσθέστε εργάσιμες ημέρες
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// προσθέστε Σαββατοκύριακο
var td22 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    0,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

costAssignment.TimephasedData.Add(td11);
costAssignment.TimephasedData.Add(td22);

Console.WriteLine("Print assignment timephased data:");
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
    foreach (var tds in assignment.TimephasedData)
    {
        Console.WriteLine("  Uid: " + tds.Uid);
        Console.WriteLine("  Start: " + tds.Start);
        Console.WriteLine("  Finish: " + tds.Finish);
        Console.WriteLine("  Type: " + tds.TimephasedDataType);
        Console.WriteLine("  Unit: " + tds.Unit);
        Console.WriteLine("  Value: " + tds.Value);
        Console.WriteLine("  ValueToCost: " + tds.ValueToCost);
        Console.WriteLine("  ValueToDuration: " + tds.ValueToDuration);
        Console.WriteLine("  ValueToUnits: " + tds.ValueToUnits);
        Console.WriteLine();
    }
}

project.Recalculate();
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


