---
title: "Group sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Group sınıfı. Bir grup tanımını temsil eder. Group nesnesi ResourceGroups koleksiyonunun veya TaskGroups koleksiyonunun bir üyesidir."
type: docs
weight: 770
url: /tr/net/aspose.tasks/group/
---
## Group class

Bir grup tanımını temsil eder. Group nesnesi ResourceGroups koleksiyonunun veya TaskGroups koleksiyonunun bir üyesidir.

```csharp
public class Group
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Group](group/)() | `Group` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [GroupAssignments](../../aspose.tasks/group/groupassignments/) { get; set; } | Atamaların görevler yerine gruplanıp gruplanmayacağını belirten bir değeri alır veya ayarlar. |
| [GroupCriteria](../../aspose.tasks/group/groupcriteria/) { get; set; } | Bir grup tanımındaki alanları temsil eden GroupCriteria koleksiyonunu alır veya ayarlar. |
| [MaintainHierarchy](../../aspose.tasks/group/maintainhierarchy/) { get; set; } | Grup içindeki alt görevler için özet görevlerin tüm seviyelerinin gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. |
| [Name](../../aspose.tasks/group/name/) { get; set; } | Group nesnesinin adını alır veya ayarlar. |
| [ShowInMenu](../../aspose.tasks/group/showinmenu/) { get; set; } | Project'in grup adını Şerit'teki Grup açılır listesinde gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. |
| [ShowSummary](../../aspose.tasks/group/showsummary/) { get; set; } | Grup için özet satırların gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. |
| [Uid](../../aspose.tasks/group/uid/) { get; } | Bir grubun benzersiz tanımlayıcısını alır. |

## Örnekler

Gruplarla nasıl çalışılacağını gösterir.

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

Projeye grup eklemenin nasıl yapılacağını gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


