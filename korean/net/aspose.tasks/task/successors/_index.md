---
title: "Task.Successors"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 이 Task 객체의 모든 후속 작업을 포함하는 TaskCollection 객체를 가져옵니다"
type: docs
weight: 1200
url: /ko/net/aspose.tasks/task/successors/
---
## Task.Successors property

이 Task 객체의 모든 후속 작업을 포함하는 [`TaskCollection`](../../taskcollection/) 객체를 가져옵니다.

```csharp
public TaskCollection Successors { get; }
```

### 반환 값

[`TaskCollection`](../../taskcollection/) 클래스의 읽기 전용 인스턴스입니다.

## 예제

작업의 후속 작업을 읽는 방법을 보여줍니다.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### 또 보기

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


