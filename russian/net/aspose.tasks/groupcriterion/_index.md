---
title: "Класс GroupCriterion"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.GroupCriterion. Представляет критерий в определении группы. Объект GroupCriterion является членом коллекции GroupCriterionCollection."
type: docs
weight: 790
url: /ru/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

Представляет критерий в определении группы. Объект GroupCriterion является членом коллекции [`GroupCriterionCollection`](../groupcriterioncollection/).

```csharp
public class GroupCriterion
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | Получает или задает значение, указывающее, сортируется ли поле, используемое в качестве критерия в определении группы, по возрастанию. False, если поле сортируется по убыванию. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | Получает или задает цвет фона ячейки для поля, используемого в качестве критерия в определении группы. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | Получает или задает поле, по которому производится группировка. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | Получает или задает шрифт для критерия в определении группы. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | Получает или задает цвет шрифта для поля, используемого в качестве критерия в определении группы. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | Получает или задает интервал для поля, используемого в качестве критерия в определении группы. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | Получает или задает тип группировки для поля, используемого в качестве критерия в определении группы. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | Получает или задает шаблон ячейки для поля, используемого в качестве критерия в определении группы. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | Получает или задает начало интервалов для поля, используемого в качестве критерия в определении группы. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | Служит хеш-функцией для определённого типа. |

## Примеры

Показывает, как читать свойства группового критерия.

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

// читать фоновый шаблон критерия  
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

Показывает, как добавить группы в проект.

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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


