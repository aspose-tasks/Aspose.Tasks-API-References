---
title: "Tsk.LateFinish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 프로젝트 종료를 지연시키지 않고 마칠 수 있는 가장 최신 날짜"
type: docs
weight: 730
url: /ko/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

작업이 프로젝트 완료를 지연시키지 않고 마칠 수 있는 가장 최신 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## 예제

Tsk.LateFinish 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


