---
title: "ResourceAssignment.Guid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 속성. 이 할당에 대한 고유 식별자를 가져오거나 설정합니다."
type: docs
weight: 290
url: /ko/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

이 할당에 대한 고유 식별자를 가져오거나 설정합니다.

```csharp
public Guid? Guid { get; set; }
```

## 예제

리소스 할당 GUID를 읽는 방법을 보여줍니다.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### 또 보기

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


