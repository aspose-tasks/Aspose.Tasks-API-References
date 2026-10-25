---
title: "类 GroupCriterion"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.GroupCriterion 类。 表示分组定义中的一个准则。GroupCriterion 对象是 GroupCriterionCollection 集合的成员。"
type: docs
weight: 790
url: /zh/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

表示分组定义中的一个准则。GroupCriterion 对象是 [`GroupCriterionCollection`](../groupcriterioncollection/) 集合的成员。

```csharp
public class GroupCriterion
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | 获取或设置一个值，指示在分组定义中用作准则的字段是否按升序排序。如果字段按降序排序，则为 false。 |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | 获取或设置在分组定义中用作准则的字段的单元格背景颜色。 |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | 获取或设置用于分组的字段。 |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | 获取或设置分组定义中准则的字体。 |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | 获取或设置在分组定义中用作准则的字段的字体颜色。 |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | 获取或设置在分组定义中用作准则的字段的间隔。 |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | 获取或设置在分组定义中用作准则的字段的分组类型。 |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | 获取或设置用于组定义中作为条件的字段的单元格模式。 |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | 获取或设置用于组定义中作为条件的字段的区间起始值。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | 作为特定类型的哈希函数。 |

## 示例

展示如何读取组准则的属性。

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

// 读取准则的背景模式。
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

展示如何向项目添加组。

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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


