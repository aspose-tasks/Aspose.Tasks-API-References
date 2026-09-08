---
title: "Class GroupCriterion"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GroupCriterion class. Vertegenwoordigt een criterium in een groepsdefinitie. Het GroupCriterion-object is een lid van de GroupCriterionCollection-collectie."
type: docs
weight: 790
url: /nl/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

Vertegenwoordigt een criterium in een groepsdefinitie. Het GroupCriterion-object is een lid van de [`GroupCriterionCollection`](../groupcriterioncollection/) collectie.

```csharp
public class GroupCriterion
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een veld dat als criterium in een groepsdefinitie wordt gebruikt, gesorteerd is in oplopende volgorde. Onwaar als het veld gesorteerd is in aflopende volgorde. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | Haalt op of stelt de kleur van de celachtergrond in voor een veld dat als criterium in een groepsdefinitie wordt gebruikt. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | Haalt op of stelt het veld in waarop gegroepeerd wordt. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | Haalt op of stelt het lettertype in voor een criterium in een groepsdefinitie. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | Haalt op of stelt de kleur van het lettertype in voor een veld dat als criterium in een groepsdefinitie wordt gebruikt. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | Haalt op of stelt het interval in voor een veld dat als criterium in een groepsdefinitie wordt gebruikt. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | Haalt op of stelt het type groepering in voor een veld dat als criterium in een groepsdefinitie wordt gebruikt. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | Haalt het patroon van de cel op of stelt het in voor een veld dat wordt gebruikt als criterium in een groepsdefinitie. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | Haalt het begin van de intervallen op of stelt het in voor een veld dat wordt gebruikt als criterium in een groepsdefinitie. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | Dient als een hash-functie voor een bepaald type. |

## Voorbeelden

Toont hoe de eigenschappen van een groepscriterium gelezen kunnen worden.

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

// lees het achtergrondpatroon van het criterium
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

Toont hoe groepen aan een project toe te voegen.

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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


