---
title: "ResourceAssignment.Delete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. 프로젝트 할당 컬렉션에서 리소스 할당을 삭제합니다"
type: docs
weight: 680
url: /ko/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

프로젝트 할당 컬렉션에서 리소스 할당을 삭제합니다.

```csharp
public void Delete()
```

## 예제

리소스 할당을 삭제하는 방법을 보여줍니다.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### 또 보기

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


