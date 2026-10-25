---
title: "Tsk.FinishText"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Tsk field. Возвращает текст завершения задачи"
type: docs
weight: 410
url: /ru/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

Возвращает текст завершения задачи.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.FinishText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


