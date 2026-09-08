---
title: "Task.OutlineOutdent"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 개요에서 작업을 승격합니다."
type: docs
weight: 1390
url: /ko/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

개요에서 작업을 승격시킵니다.

```csharp
public void OutlineOutdent()
```

## 예제

작업을 내어쓰기하는 방법을 보여줍니다.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// 작업을 내어쓰기
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


