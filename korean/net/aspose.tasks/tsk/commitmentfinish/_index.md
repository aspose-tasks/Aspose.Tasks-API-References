---
title: "Tsk.CommitmentFinish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 전달의 완료 날짜입니다.  XML 형식에 대해서만 읽기가 지원됩니다."
type: docs
weight: 170
url: /ko/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

전달의 종료 날짜. 읽기는 XML 형식만 지원됩니다.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## 예제

Tsk.CommitmentFinish 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


