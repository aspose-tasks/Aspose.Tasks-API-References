---
title: "클래스 GroupCriterion"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GroupCriterion 클래스. 그룹 정의에서 기준을 나타냅니다. GroupCriterion 객체는 GroupCriterionCollection 컬렉션의 멤버입니다."
type: docs
weight: 790
url: /ko/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

그룹 정의에서 기준을 나타냅니다. GroupCriterion 객체는 [`GroupCriterionCollection`](../groupcriterioncollection/) 컬렉션의 멤버입니다.

```csharp
public class GroupCriterion
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | 그룹 정의에서 기준으로 사용되는 필드가 오름차순으로 정렬되는지 여부를 나타내는 값을 가져오거나 설정합니다. 필드가 내림차순으로 정렬된 경우 false입니다. |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | 그룹 정의에서 기준으로 사용되는 필드의 셀 배경 색상을 가져오거나 설정합니다. |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | 그룹화에 사용되는 필드를 가져오거나 설정합니다. |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | 그룹 정의에서 기준에 대한 글꼴을 가져오거나 설정합니다. |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | 그룹 정의에서 기준으로 사용되는 필드의 글꼴 색상을 가져오거나 설정합니다. |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | 그룹 정의에서 기준으로 사용되는 필드의 간격을 가져오거나 설정합니다. |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | 그룹 정의에서 기준으로 사용되는 필드의 그룹화 유형을 가져오거나 설정합니다. |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | 그룹 정의에서 기준으로 사용되는 필드의 셀 패턴을 가져오거나 설정합니다. |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | 그룹 정의에서 기준으로 사용되는 필드의 구간 시작을 가져오거나 설정합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | 특정 유형에 대한 해시 함수 역할을 합니다. |

## 예제

그룹 기준의 속성을 읽는 방법을 보여줍니다.

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

// 기준의 배경 패턴을 읽습니다
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
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


