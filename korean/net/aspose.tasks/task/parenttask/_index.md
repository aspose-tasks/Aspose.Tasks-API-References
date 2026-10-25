---
title: "Task.ParentTask"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 작업의 상위 작업을 가져옵니다"
type: docs
weight: 940
url: /ko/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

작업의 상위 작업을 가져옵니다.

```csharp
public Task ParentTask { get; }
```

## 예제

작업의 상위 작업을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


