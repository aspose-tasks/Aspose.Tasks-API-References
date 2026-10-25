---
title: "Class GroupCriterion"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GroupCriterion sınıfı. Bir grup tanımındaki kriteri temsil eder. GroupCriterion nesnesi, GroupCriterionCollection koleksiyonunun bir üyesidir."
type: docs
weight: 790
url: /tr/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

Bir grup tanımındaki kriteri temsil eder. GroupCriterion nesnesi, [`GroupCriterionCollection`](../groupcriterioncollection/) koleksiyonunun bir üyesidir.

```csharp
public class GroupCriterion
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | Bir grup tanımında kriter olarak kullanılan bir alanın artan sırada sıralanıp sıralanmadığını gösteren bir değeri alır veya ayarlar. Alan azalan sırada sıralanmışsa false döner. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | Bir grup tanımında kriter olarak kullanılan bir alanın hücre arka plan rengini alır veya ayarlar. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | Gruplandırılan alanı alır veya ayarlar. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | Bir grup tanımındaki kriter için yazı tipini alır veya ayarlar. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | Bir grup tanımında kriter olarak kullanılan bir alanın yazı tipi rengini alır veya ayarlar. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | Bir grup tanımında kriter olarak kullanılan bir alanın aralığını alır veya ayarlar. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | Bir grup tanımında kriter olarak kullanılan bir alanın grup türünü alır veya ayarlar. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | Bir grup tanımında ölçüt olarak kullanılan alan için hücrenin desenini alır veya ayarlar. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | Bir grup tanımında ölçüt olarak kullanılan alan için aralıkların başlangıcını alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | Belirli bir tür için hash işlevi olarak hizmet verir. |

## Örnekler

Bir grup kriterinin özelliklerini nasıl okuyacağınızı gösterir.

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

// Kriterin arka plan desenini okuyun.
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
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


