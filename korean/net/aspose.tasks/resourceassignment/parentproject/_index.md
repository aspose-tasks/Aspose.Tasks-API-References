---
title: "ResourceAssignment.ParentProject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 속성. 이 할당에 대한 상위 프로젝트를 가져옵니다."
type: docs
weight: 420
url: /ko/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

이 할당에 대한 상위 프로젝트를 가져옵니다.

```csharp
public Project ParentProject { get; }
```

## 예제

리소스 할당의 상위 프로젝트를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// 기본 프로젝트 시간 단위 유형을 사용하여 할당 기간을 설정합니다.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### 또 보기

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


