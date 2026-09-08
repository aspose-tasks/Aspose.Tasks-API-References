---
title: "클래스 Group"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Group 클래스. 그룹 정의를 나타냅니다. Group 객체는 ResourceGroups 컬렉션 또는 TaskGroups 컬렉션의 구성원입니다."
type: docs
weight: 770
url: /ko/net/aspose.tasks/group/
---
## Group class

그룹 정의를 나타냅니다. Group 객체는 ResourceGroups 컬렉션 또는 TaskGroups 컬렉션의 구성원입니다.

```csharp
public class Group
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Group](group/)() | `Group` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [GroupAssignments](../../aspose.tasks/group/groupassignments/) { get; set; } | 작업 대신 할당을 그룹화해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [GroupCriteria](../../aspose.tasks/group/groupcriteria/) { get; set; } | 그룹 정의의 필드를 나타내는 GroupCriteria 컬렉션을 가져오거나 설정합니다. |
| [MaintainHierarchy](../../aspose.tasks/group/maintainhierarchy/) { get; set; } | 그룹 내 하위 작업에 대한 요약 작업의 모든 레벨을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Name](../../aspose.tasks/group/name/) { get; set; } | Group 객체의 이름을 가져오거나 설정합니다. |
| [ShowInMenu](../../aspose.tasks/group/showinmenu/) { get; set; } | 리본의 Group 드롭다운 목록에 프로젝트가 그룹 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowSummary](../../aspose.tasks/group/showsummary/) { get; set; } | 그룹에 대한 요약 행을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Uid](../../aspose.tasks/group/uid/) { get; } | 그룹의 고유 식별자를 가져옵니다. |

## 예제

그룹 작업 방법을 보여줍니다.

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

프로젝트에 그룹을 추가하는 방법을 보여줍니다.

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

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


