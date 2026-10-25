---
title: "Tsk.EarlyStart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Самая ранняя дата, когда задача может начаться, основываясь на датах раннего начала предшествующих и последующих задач и других ограничениях"
type: docs
weight: 340
url: /ru/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

Самая ранняя дата, когда задача может начаться, исходя из ранних дат начала предшествующих и последующих задач и других ограничений.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.EarlyStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


