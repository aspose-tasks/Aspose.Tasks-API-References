---
title: "Tsk.StartText"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Возвращает начальный текст задачи."
type: docs
weight: 1030
url: /ru/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

Возвращает начальный текст задачи.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.StartText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


