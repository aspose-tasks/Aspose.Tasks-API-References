---
title: "Tsk.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Gerçek işin korunduğu süre. Okuma yalnızca XML formatı için desteklenir."
type: docs
weight: 100
url: /tr/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

Gerçek işin korunduğu süre. Okuma yalnızca XML formatı için desteklenir.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## Örnekler

Tsk.ActualWorkProtected özelliğini nasıl okuyup/yazacağınızı gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


