---
title: "Κλάση Group"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Group. Αντιπροσωπεύει έναν ορισμό ομάδας. Ένα αντικείμενο Group είναι μέλος της συλλογής ResourceGroups ή της συλλογής TaskGroups."
type: docs
weight: 770
url: /el/net/aspose.tasks/group/
---
## Group class

Αντιπροσωπεύει έναν ορισμό ομάδας. Ένα αντικείμενο Group είναι μέλος της συλλογής ResourceGroups ή της συλλογής TaskGroups.

```csharp
public class Group
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Group](group/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `Group`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [GroupAssignments](../../aspose.tasks/group/groupassignments/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν οι αναθέσεις πρέπει να ομαδοποιούνται αντί για εργασίες. |
| [GroupCriteria](../../aspose.tasks/group/groupcriteria/) { get; set; } | Λαμβάνει ή ορίζει μια συλλογή GroupCriteria που αντιπροσωπεύει τα πεδία σε έναν ορισμό ομάδας. |
| [MaintainHierarchy](../../aspose.tasks/group/maintainhierarchy/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται όλα τα επίπεδα των εργασιών σύνοψης για τις υποεργασίες εντός της ομάδας. |
| [Name](../../aspose.tasks/group/name/) { get; set; } | Λαμβάνει ή ορίζει ένα όνομα αντικειμένου Group. |
| [ShowInMenu](../../aspose.tasks/group/showinmenu/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το Project εμφανίζει το όνομα της ομάδας στη λίστα επιλογής Group στην κορδέλα. |
| [ShowSummary](../../aspose.tasks/group/showsummary/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν οι γραμμές σύνοψης εμφανίζονται για την ομάδα. |
| [Uid](../../aspose.tasks/group/uid/) { get; } | Λαμβάνει ένα μοναδικό αναγνωριστικό μιας ομάδας. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με ομάδες.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Uid: " + group.Uid);
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Is Task Group Maintain Hierarchy?: " + group.MaintainHierarchy);
Console.WriteLine("Is Task Group Show In Menu?: " + group.ShowInMenu);
Console.WriteLine("Is Task Group Show Summary?: " + group.ShowSummary);
Console.WriteLine("Is Task Group should groups Assignments instead of Tasks?: " + group.GroupAssignments);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);
Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");

foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Task Criterion Field: " + criterion.Field);
    Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
    Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
    Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

    Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
    Console.WriteLine("Font Size: " + criterion.Font.Size);
    Console.WriteLine("Font Style: " + criterion.Font.Style);
    Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
}
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


