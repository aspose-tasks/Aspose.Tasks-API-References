---
title: "Tsk.EarlyFinish"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Самая ранняя дата, когда задача может завершиться, исходя из дат раннего завершения предшествующих и последующих задач, других ограничений и любой задержки выравнивания"
type: docs
weight: 330
url: /ru/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

Самая ранняя дата, когда задача может быть завершена, исходя из ранних дат завершения предшествующих и последующих задач, других ограничений и любой задержки выравнивания.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.EarlyFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


