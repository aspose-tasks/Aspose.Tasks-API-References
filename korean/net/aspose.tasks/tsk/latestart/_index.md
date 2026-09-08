---
title: "Tsk.LateStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 프로젝트 종료를 지연시키지 않고 시작할 수 있는 가장 최신 날짜"
type: docs
weight: 740
url: /ko/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

작업이 프로젝트 완료를 지연시키지 않고 시작할 수 있는 가장 최신 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## 예제

Tsk.LateStart 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


