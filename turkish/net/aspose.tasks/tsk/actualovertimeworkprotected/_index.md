---
title: "Tsk.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Gerçek fazla mesai çalışmasının korunduğu süre"
type: docs
weight: 70
url: /tr/net/aspose.tasks/tsk/actualovertimeworkprotected/
---
## Tsk.ActualOvertimeWorkProtected field

Gerçek fazla mesai çalışmasının korunduğu süre.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWorkProtected;
```

## Örnekler

Tsk.ActualOvertimeWorkProtected özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + task.Get(Tsk.ActualOvertimeWorkProtected));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


