---
title: "Tsk.IsMarked"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Показывает, помечена ли задача для дальнейших действий или какого-либо типа идентификации"
type: docs
weight: 620
url: /ru/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

Показывает, помечена ли задача для дальнейших действий или какой-либо идентификации.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## Примечания

Применяется только к формату файлов mpp.

## Примеры

Показывает, как читать/записывать свойство Tsk.IsMarked.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


