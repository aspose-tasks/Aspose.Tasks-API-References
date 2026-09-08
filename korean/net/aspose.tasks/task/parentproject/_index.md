---
title: "Task.ParentProject"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 작업의 상위 프로젝트를 가져옵니다."
type: docs
weight: 930
url: /ko/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

작업의 상위 프로젝트를 가져옵니다.

```csharp
public Project ParentProject { get; }
```

## 비고

이러한 속성을 업데이트하려면 Project.UpdateReferences를 호출하십시오.

## 예제

작업의 상위 프로젝트를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// 기본 프로젝트 시간 단위 유형을 사용하여 작업의 기간을 설정합니다.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### 또 보기

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


