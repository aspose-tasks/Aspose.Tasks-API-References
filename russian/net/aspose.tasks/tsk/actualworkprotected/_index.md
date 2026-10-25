---
title: "Tsk.ActualWorkProtected"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Продолжительность, в течение которой фактическая работа защищена. Чтение поддерживается только для формата XML"
type: docs
weight: 100
url: /ru/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

Продолжительность, в течение которой фактическая работа защищена. Чтение поддерживается только для формата XML.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


