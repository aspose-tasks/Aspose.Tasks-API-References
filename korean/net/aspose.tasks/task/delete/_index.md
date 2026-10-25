---
title: "Task.Delete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 부모 프로젝트 작업 컬렉션 및 모든 할당에서 작업을 삭제합니다."
type: docs
weight: 1320
url: /ko/net/aspose.tasks/task/delete/
---
## Task.Delete method

상위 프로젝트 작업 컬렉션 및 해당 작업의 모든 할당에서 작업을 삭제합니다.

```csharp
public void Delete()
```

## 예제

작업을 삭제하는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// 작업을 삭제
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


