---
title: "Tsk.DurationText"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Tsk field. Возвращает текст длительности задачи"
type: docs
weight: 310
url: /ru/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

Возвращает текст продолжительности задачи.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.DurationText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


