---
title: "Classe Group"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Group classe. Rappresenta una definizione di gruppo. Un oggetto Group è un membro della collezione ResourceGroups o della collezione TaskGroups"
type: docs
weight: 770
url: /it/net/aspose.tasks/group/
---
## Group class

Rappresenta una definizione di gruppo. Un oggetto Group è membro della collezione ResourceGroups o della collezione TaskGroups.

```csharp
public class Group
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Group](group/)() | Inizializza una nuova istanza della classe `Group`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [GroupAssignments](../../aspose.tasks/group/groupassignments/) { get; set; } | Ottiene o imposta un valore che indica se le assegnazioni devono essere raggruppate invece dei task. |
| [GroupCriteria](../../aspose.tasks/group/groupcriteria/) { get; set; } | Ottiene o imposta una collezione GroupCriteria che rappresenta i campi in una definizione di gruppo. |
| [MaintainHierarchy](../../aspose.tasks/group/maintainhierarchy/) { get; set; } | Ottiene o imposta un valore che indica se mostrare tutti i livelli dei task di riepilogo per i sotto-task all'interno del gruppo. |
| [Name](../../aspose.tasks/group/name/) { get; set; } | Ottiene o imposta il nome di un oggetto Group. |
| [ShowInMenu](../../aspose.tasks/group/showinmenu/) { get; set; } | Ottiene o imposta un valore che indica se Project mostra il nome del gruppo nell'elenco a discesa Group nella barra multifunzione. |
| [ShowSummary](../../aspose.tasks/group/showsummary/) { get; set; } | Ottiene o imposta un valore che indica se le righe di riepilogo sono visualizzate per il gruppo. |
| [Uid](../../aspose.tasks/group/uid/) { get; } | Ottiene un identificatore univoco di un gruppo. |

## Esempi

Mostra come lavorare con i gruppi.

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

Mostra come aggiungere gruppi a un progetto.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


