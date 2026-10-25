---
title: "Tsk.PreleveledFinish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 리소스 레벨링이 수행되기 전 작업의 완료 날짜"
type: docs
weight: 910
url: /ko/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

리소스 레벨링이 수행되기 전 작업의 완료 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## 예제

Tsk.PreleveledFinish 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


