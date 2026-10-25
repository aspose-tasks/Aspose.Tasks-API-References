---
title: "GroupCriterion.Ascending"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GroupCriterion 속성. 그룹 정의에서 기준으로 사용되는 필드가 오름차순으로 정렬되는지 여부를 나타내는 값을 가져오거나 설정합니다. 필드가 내림차순으로 정렬된 경우 false입니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/groupcriterion/ascending/
---
## GroupCriterion.Ascending property

그룹 정의에서 기준으로 사용되는 필드가 오름차순으로 정렬되는지 여부를 나타내는 값을 가져오거나 설정합니다. 필드가 내림차순으로 정렬된 경우 false입니다.

```csharp
public bool Ascending { get; set; }
```

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

### 또 보기

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)


