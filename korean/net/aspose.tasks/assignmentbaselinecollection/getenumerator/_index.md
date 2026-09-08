---
title: "AssignmentBaselineCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 참조"
description: "AssignmentBaselineCollection 메서드. 이 컬렉션에 대한 열거자를 반환합니다"
type: docs
weight: 50
url: /ko/net/aspose.tasks/assignmentbaselinecollection/getenumerator/
---
## AssignmentBaselineCollection.GetEnumerator method

이 컬렉션에 대한 열거자를 반환합니다.

```csharp
public IEnumerator<AssignmentBaseline> GetEnumerator()
```

### 반환 값

이 컬렉션에 대한 열거자.

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


