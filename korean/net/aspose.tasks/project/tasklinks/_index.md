---
title: "Project.TaskLinks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. TaskLinkCollection 객체를 가져옵니다."
type: docs
weight: 930
url: /ko/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

[`TaskLinkCollection`](../../tasklinkcollection/) 객체를 가져옵니다.

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## 예제

작업 링크를 만드는 방법을 보여줍니다.

```csharp
var project = new Project();

// 새 작업 추가
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// 작업 연결
project.TaskLinks.Add(pred, succ);

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Predecessor Task: " + link.PredTask);
    Console.WriteLine("Successor Task: " + link.SuccTask);
    Console.WriteLine("LagFormat: " + link.LagFormat);
    Console.WriteLine("LinkType: " + link.LinkType);
    Console.WriteLine("LinkLag: " + link.LinkLag);
    Console.WriteLine("CrossProjectName: " + link.CrossProjectName);
    Console.WriteLine("IsCrossProject: " + link.IsCrossProject);
}
```

### 또 보기

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


