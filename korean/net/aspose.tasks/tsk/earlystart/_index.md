---
title: "Tsk.EarlyStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 선행 및 후속 작업의 조기 시작 날짜와 기타 제약 조건을 기반으로 작업이 시작될 수 있는 가장 이른 날짜입니다."
type: docs
weight: 340
url: /ko/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

선행 및 후속 작업의 조기 시작 날짜와 기타 제약 조건을 기반으로 작업이 시작될 수 있는 가장 이른 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## 예제

Tsk.EarlyStart 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


