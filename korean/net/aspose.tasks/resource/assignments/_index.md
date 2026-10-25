---
title: "Resource.Assignments"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 속성. 이 객체에 대한 리소스 할당 컬렉션을 가져옵니다."
type: docs
weight: 120
url: /ko/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

이 객체에 대한 리소스 할당 컬렉션을 가져옵니다.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## 예제

리소스 할당을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

foreach (var resource in project.Resources)
{
    foreach (var assignment in resource.Assignments)
    {
        Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
        Console.WriteLine("Assignment's task name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
    }
}
```

### 또 보기

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


