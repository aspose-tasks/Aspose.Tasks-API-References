---
title: "ResourceAssignment.Baselines"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment property. AssignmentBaselineCollection 객체를 가져옵니다. 할당과 연관된 기준값들의 컬렉션"
type: docs
weight: 120
url: /ko/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

AssignmentBaselineCollection 객체를 가져옵니다. 할당과 연결된 기준값 컬렉션입니다.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## 예제

할당의 기준값에 접근하는 방법을 보여줍니다.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

project.SetBaseline(BaselineType.Baseline);

foreach (var assignmentBaseline in resourceAssignment.Baselines)
{
    Console.WriteLine("Baseline Start: {0}", assignmentBaseline.Start);
    Console.WriteLine("Baseline Finish: {0}", assignmentBaseline.Finish);
}
```

### 또 보기

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


