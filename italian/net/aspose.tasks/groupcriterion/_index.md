---
title: "Classe GroupCriterion"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.GroupCriterion class. Rappresenta un criterio in una definizione di gruppo. L'oggetto GroupCriterion è un membro della collezione GroupCriterionCollection."
type: docs
weight: 790
url: /it/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

Rappresenta un criterio in una definizione di gruppo. L'oggetto GroupCriterion è un membro della collezione [`GroupCriterionCollection`](../groupcriterioncollection/).

```csharp
public class GroupCriterion
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | Ottiene o imposta un valore che indica se un campo utilizzato come criterio in una definizione di gruppo è ordinato in ordine crescente. False se il campo è ordinato in ordine decrescente. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | Ottiene o imposta il colore dello sfondo della cella per un campo utilizzato come criterio in una definizione di gruppo. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | Ottiene o imposta il campo per il quale si effettua il raggruppamento. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | Ottiene o imposta il carattere per un criterio in una definizione di gruppo. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | Ottiene o imposta il colore del carattere per un campo utilizzato come criterio in una definizione di gruppo. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | Ottiene o imposta l'intervallo per un campo utilizzato come criterio in una definizione di gruppo. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | Ottiene o imposta il tipo di raggruppamento per un campo utilizzato come criterio in una definizione di gruppo. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | Ottiene o imposta il modello della cella per un campo utilizzato come criterio in una definizione di gruppo. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | Ottiene o imposta l'inizio degli intervalli per un campo utilizzato come criterio in una definizione di gruppo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | Funziona come funzione hash per un tipo specifico. |

## Esempi

Mostra come leggere le proprietà di un criterio di gruppo.

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

// leggi il modello di sfondo del criterio
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
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


