---
title: "열거형 TaskLinkType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskLinkType 열거형. 작업 종속성 유형을 지정합니다"
type: docs
weight: 2440
url: /ko/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

작업 종속성 유형을 지정합니다.

```csharp
public enum TaskLinkType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| FinishToFinish | `0` | Finish-Finish 관계 |
| FinishToStart | `1` | Finish-Start 관계 |
| StartToFinish | `2` | Start-Finish 관계 |
| StartToStart | `3` | Start-Start 관계 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


