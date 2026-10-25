---
title: "Task.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 이 작업의 모든 하위 작업을 재귀적으로 수집합니다"
type: docs
weight: 1400
url: /ko/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

이 작업의 모든 하위 작업을 재귀적으로 수집합니다.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### 반환 값

이 작업의 하위 작업 목록입니다.

## 예제

하위 작업을 반복하는 방법을 보여줍니다.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


