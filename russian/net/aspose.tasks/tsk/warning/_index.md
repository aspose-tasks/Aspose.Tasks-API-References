---
title: "Tsk.Warning"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Представляет флаг, указывающий, что у задачи есть несоответствия расписания"
type: docs
weight: 1120
url: /ru/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

Представляет флаг, который указывает, что у задачи есть расхождения в расписании.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## Примеры

Показывает, как прочитать предупреждение задачи.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


