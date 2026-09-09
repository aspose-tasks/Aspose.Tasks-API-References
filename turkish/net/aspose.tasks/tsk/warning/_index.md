---
title: "Tsk.Warning"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevin zaman çizelgesi tutarsızlıkları olduğunu gösteren bayrağı temsil eder"
type: docs
weight: 1120
url: /tr/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

Görevin zamanlama tutarsızlıkları olduğunu gösteren bayrağı temsil eder.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## Örnekler

Bir görev uyarısının nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


