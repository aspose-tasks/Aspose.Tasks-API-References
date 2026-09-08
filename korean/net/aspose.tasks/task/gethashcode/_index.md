---
title: "Task.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 이 Task에 대한 해시 코드 값을 반환합니다."
type: docs
weight: 1350
url: /ko/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

이 Task에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

작업의 해시 코드를 얻는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// 작업의 해시 코드는 작업의 UID와 이름을 기반으로 합니다.
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


