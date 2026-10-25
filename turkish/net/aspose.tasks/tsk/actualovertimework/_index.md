---
title: "Tsk.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk field. Görevlere atanan kaynaklar tarafından zaten yapılan gerçek fazla mesai miktarı"
type: docs
weight: 60
url: /tr/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

Görevlere atanan kaynaklar tarafından zaten yapılan fazla mesai çalışmasının gerçek miktarı.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## Örnekler

Tsk.ActualOvertimeWork özelliğini okuma/yazma nasıl gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


