---
title: "Tsk.Type"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin türü."
type: docs
weight: 1100
url: /tr/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

Bir görevin türü.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## Örnekler

Tsk.Type özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


