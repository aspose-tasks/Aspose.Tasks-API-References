---
title: "Tsk.Warning"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 일정 불일치가 있음을 나타내는 플래그를 나타냅니다."
type: docs
weight: 1120
url: /ko/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

작업에 일정 불일치가 있음을 나타내는 플래그를 나타냅니다.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## 예제

작업 경고를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


