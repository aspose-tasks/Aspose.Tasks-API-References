---
title: "Tsk.StartSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 조기 시작일과 늦은 시작일 사이의 기간"
type: docs
weight: 1020
url: /ko/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

조기 시작과 늦은 시작 날짜 사이의 기간.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## 예제

Tsk.StartSlackTimeSpan 속성을 읽는 방법을 보여줍니다. 이 속성은 계산되므로 일반적으로 명시적으로 설정할 필요가 없습니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


