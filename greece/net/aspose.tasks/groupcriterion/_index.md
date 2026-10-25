---
title: "Class GroupCriterion"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.GroupCriterion class. Αντιπροσωπεύει ένα κριτήριο σε ορισμό ομάδας. Το αντικείμενο GroupCriterion είναι μέλος της συλλογής GroupCriterionCollection collection"
type: docs
weight: 790
url: /el/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

Αντιπροσωπεύει ένα κριτήριο σε ορισμό ομάδας. Το αντικείμενο GroupCriterion είναι μέλος της συλλογής [`GroupCriterionCollection`](../groupcriterioncollection/) collection.

```csharp
public class GroupCriterion
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας είναι ταξινομημένο σε αύξουσα σειρά. Ψευδές εάν το πεδίο είναι ταξινομημένο σε φθίνουσα σειρά. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα του φόντου του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | Λαμβάνει ή ορίζει το πεδίο με το οποίο γίνεται ομαδοποίηση. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | Λαμβάνει ή ορίζει τη γραμματοσειρά για ένα κριτήριο σε ορισμό ομάδας. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα της γραμματοσειράς για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | Λαμβάνει ή ορίζει το διάστημα για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο ομαδοποίησης για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | Λαμβάνει ή ορίζει το μοτίβο του κελιού για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | Λαμβάνει ή ορίζει την αρχή των διαστημάτων για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | Λειτουργεί ως συνάρτηση κατακερματισμού για έναν συγκεκριμένο τύπο. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις ιδιότητες ενός κριτηρίου ομάδας.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// Διαβάστε το υπόβαθρο του προτύπου του κριτηρίου.
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

Δείχνει πώς να προσθέσετε ομάδες σε ένα έργο.

```csharp
var p = new Project();

{
    var group = new Group();
    group.Name = "My new task group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.TaskDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 13F, FontStyles.Italic);
    criterion.GroupOn = GroupOn.DurationMinutes;
    criterion.StartAt = 5;
    criterion.GroupInterval = 3D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.TaskPercentComplete;
    criterion2.Font = new FontDescriptor("Bodoni MT", 17, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Pct199;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Green;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.TaskGroups.Add(group);
}

{
    var group = new Group();
    group.Name = "My new resource group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.ResourceDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 11F, FontStyles.Bold);
    criterion.GroupOn = GroupOn.DurationHours;
    criterion.StartAt = 1;
    criterion.GroupInterval = 2D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.ResourceCost;
    criterion2.Font = new FontDescriptor("Bodoni MT", 12, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Interval;
    criterion2.StartAt = 1D;
    criterion2.GroupInterval = 10D;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Magenta;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.ResourceGroups.Add(group);
}

p.Save(OutDir + "output_CreateGroup.mpp", new MPPSaveOptions() { WriteGroups = true });
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


