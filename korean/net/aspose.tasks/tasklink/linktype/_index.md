---
title: "TaskLink.LinkType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskLink 속성. 링크 유형을 가져오거나 설정합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

링크 유형을 가져오거나 설정합니다.

```csharp
public TaskLinkType LinkType { get; set; }
```

## 예제

작업 링크의 링크 유형을 가져오거나 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 새 작업 추가
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// 링크 유형이 Start to Start으로 설정된 작업을 연결합니다
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### 또 보기

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


