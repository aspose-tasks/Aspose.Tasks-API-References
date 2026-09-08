---
title: "Tsk.IsRecurring"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 반복 작업 시리즈의 일부인지 여부를 결정합니다"
type: docs
weight: 670
url: /ko/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

작업이 반복 작업 시리즈의 일부인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## 예제

Tsk.IsRecurring 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


