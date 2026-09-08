---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 조기 종료와 늦은 종료 날짜 사이의 기간"
type: docs
weight: 400
url: /ko/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

조기 종료와 후기 종료 날짜 사이의 기간.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## 예제

Tsk.FinishSlackTimeSpan 속성을 읽는 방법을 보여줍니다. 이 속성은 계산되므로 일반적으로 명시적으로 설정할 필요가 없습니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


