---
title: "Project.CriticalPath"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 이 프로젝트의 Critical Path를 구성하는 Critical 작업 목록을 포함하는 컬렉션을 가져옵니다. 이는 프로젝트의 작업 수를 n으로 하는 On 연산입니다."
type: docs
weight: 180
url: /ko/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

이 프로젝트의 Critical Path를 구성하는 Critical 작업 목록을 포함하는 컬렉션을 가져옵니다. 이는 프로젝트의 작업 수 n에 따라 O(n) 연산입니다.

```csharp
public TaskCollection CriticalPath { get; }
```

### 반환 값

모든 Critical 작업 목록을 나타내는 컬렉션입니다.

## 예제

프로젝트의 Critical Path를 계산하는 방법을 보여줍니다.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// 지금 Critical Path를 표시합니다.
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### 또 보기

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


