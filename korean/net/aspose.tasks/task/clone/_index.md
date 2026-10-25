---
title: "Task.Clone"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 하위 작업 없이 작업의 전체 복사본을 생성합니다"
type: docs
weight: 1310
url: /ko/net/aspose.tasks/task/clone/
---
## Task.Clone method

하위 작업 없이 작업의 전체 복사본을 생성합니다.

```csharp
public object Clone()
```

### 반환 값

작업의 복사본을 만들었습니다.

## 예제

작업을 복제하는 방법을 보여줍니다.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


