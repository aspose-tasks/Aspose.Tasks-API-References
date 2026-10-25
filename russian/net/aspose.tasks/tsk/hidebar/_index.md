---
title: "Tsk.HideBar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, скрыта ли полоса Ганта задачи при отображении в Microsoft Project."
type: docs
weight: 480
url: /ru/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Определяет, скрыта ли полоса Ганта задачи при отображении в Microsoft Project.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.HideBar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


