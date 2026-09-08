---
title: "Tsk.ActivityId"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Представляет поле идентификатора активности — уникальный идентификатор задачи, используемый в Primavera. Применяется только к проектам Primavera"
type: docs
weight: 10
url: /ru/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

Представляет поле идентификатора активности — уникальный идентификатор задачи, используемый в Primavera. (применимо только к проектам Primavera).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## Примеры

Показывает, как работать с полем ActivityId, специфичным для проектов Primavera

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// Создайте параметры сохранения Primavera и укажите, что ActivityIds не должны перезаписываться при сохранении.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


