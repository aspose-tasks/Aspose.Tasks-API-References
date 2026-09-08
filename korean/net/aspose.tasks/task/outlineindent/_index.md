---
title: "Task.OutlineIndent"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 개요에서 작업을 들여쓰기합니다."
type: docs
weight: 1380
url: /ko/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

개요에서 작업을 들여씁니다.

```csharp
public void OutlineIndent()
```

## 예제

작업을 들여쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// 작업을 들여쓰기
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


