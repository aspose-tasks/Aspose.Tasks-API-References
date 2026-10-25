---
title: "Tsk.CommitmentStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 전달의 시작 날짜입니다. 읽기는 XML 형식만 지원됩니다."
type: docs
weight: 180
url: /ko/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

전달의 시작 날짜. 읽기는 XML 형식만 지원됩니다.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## 예제

Tsk.CommitmentStart 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


