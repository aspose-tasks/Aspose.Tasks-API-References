---
title: "Tsk.PreleveledStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk field. 리소스 레벨링이 수행되기 전 작업의 시작 날짜"
type: docs
weight: 920
url: /ko/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

리소스 레벨링이 수행되기 전 작업의 시작 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## 예제

Tsk.PreleveledStart 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


