---
title: "AssignmentBaselineCollection.Count"
second_title: "Aspose.Tasks for .NET API 참조"
description: "AssignmentBaselineCollection 속성. 이 AssignmentBaselineCollection 객체에 포함된 객체 수를 가져옵니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

이 AssignmentBaselineCollection 객체에 포함된 객체 수를 가져옵니다.

```csharp
public int Count { get; }
```

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

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


