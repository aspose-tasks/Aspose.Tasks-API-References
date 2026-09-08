---
title: "Tsk.EarlyFinish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 선행 및 후속 작업의 조기 종료 날짜, 기타 제약 조건 및 레벨링 지연을 기반으로 작업이 완료될 수 있는 가장 이른 날짜"
type: docs
weight: 330
url: /ko/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

선행 및 후속 작업의 조기 종료 날짜, 기타 제약 조건 및 레벨링 지연을 기반으로 작업이 완료될 수 있는 가장 이른 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## 예제

Tsk.EarlyFinish 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


