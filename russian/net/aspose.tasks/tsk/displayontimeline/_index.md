---
title: "Tsk.DisplayOnTimeline"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Указывает, должна ли задача отображаться во временной шкале"
type: docs
weight: 290
url: /ru/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

Указывает, должна ли задача отображаться во временной шкале.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.DisplayOnTimeline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


