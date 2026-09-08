---
title: "클래스 AssignmentBaselineCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.AssignmentBaselineCollection 클래스. AssignmentBaseline 객체의 컬렉션을 나타냅니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

[`AssignmentBaseline`](../assignmentbaseline/) 객체의 컬렉션을 나타냅니다.

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | 이 AssignmentBaselineCollection 객체에 포함된 객체 수를 가져옵니다. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | 지정된 인덱스의 요소를 반환합니다. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | 이 컬렉션의 상위 [`ResourceAssignment`](../resourceassignment/)을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | ICollection의 Add 메서드에 대한 스텁 구현으로, NotSupportedException만 발생시킵니다. |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | 이 컬렉션에서 기준선을 제거합니다. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | AssignmentBaselineCollection 객체를 [`AssignmentBaseline`](../assignmentbaseline/) 객체 목록으로 변환합니다. |

## 예제

assignment baseline을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// 할당 베이스라인 정보를 읽습니다.
foreach (var assignment in project.ResourceAssignments)
{
    var baselines = assignment.Baselines;
    Console.WriteLine("Count of assignment baselines: " + baselines.Count);
    Console.WriteLine("Parent Assignment: " + baselines.ParentAssignment);
    foreach (var baseline in baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
    }

    Console.WriteLine();
}

Console.WriteLine("Delete all assignment baselines: ");

// assignment baseline 삭제
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### 또 보기

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


