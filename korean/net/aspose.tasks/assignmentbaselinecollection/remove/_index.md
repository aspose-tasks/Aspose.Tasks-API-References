---
title: "AssignmentBaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET API 참조"
description: "AssignmentBaselineCollection 메서드. 이 컬렉션에서 기준선을 제거합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

이 컬렉션에서 기준선을 제거합니다.

```csharp
public bool Remove(AssignmentBaseline item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | AssignmentBaseline | 제거할 항목입니다. |

### 반환 값

[`AssignmentBaseline`](../../assignmentbaseline/) 인스턴스가 성공적으로 제거된 경우 true; 그렇지 않으면 false

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

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


