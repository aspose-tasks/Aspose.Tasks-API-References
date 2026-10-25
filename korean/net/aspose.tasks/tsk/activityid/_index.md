---
title: "Tsk.ActivityId"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. Primavera에서 사용되는 작업 고유 식별자인 activity id 필드를 나타냅니다. Primavera 프로젝트에만 적용됩니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

활동 ID 필드를 나타냅니다 - Primavera에서 사용되는 작업의 고유 식별자입니다. (Primavera 프로젝트에만 적용됩니다.)

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## 예제

Primavera 프로젝트에 특화된 ActivityId 필드를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// Primavera 저장 옵션을 생성하고 저장 중에 ActivityId가 덮어쓰여지지 않도록 지정합니다.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


