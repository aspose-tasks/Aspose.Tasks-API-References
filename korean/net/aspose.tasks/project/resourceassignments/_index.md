---
title: "Project.ResourceAssignments"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. ResourceAssignmentCollection 객체를 가져옵니다."
type: docs
weight: 750
url: /ko/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

ResourceAssignmentCollection 객체를 가져옵니다.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## 예제

리소스 할당을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 새 작업 및 리소스를 추가합니다
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// 리소스에 원하는 작업을 할당합니다.
project.ResourceAssignments.Add(task, resource);
```

### 또 보기

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


