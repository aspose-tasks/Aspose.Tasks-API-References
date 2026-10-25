---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 프로젝트의 완료 날짜를 지연시키지 않고 작업의 종료 날짜를 연기할 수 있는 시간입니다."
type: docs
weight: 1090
url: /ko/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

프로젝트 종료 날짜를 지연시키지 않고 작업 종료 날짜를 연기할 수 있는 시간.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## 예제

Tsk.TotalSlackTimeSpan 속성을 읽는 방법을 보여줍니다. 이 속성은 계산되므로 일반적으로 명시적으로 설정할 필요가 없습니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


