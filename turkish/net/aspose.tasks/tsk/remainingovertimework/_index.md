---
title: "Tsk.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Kalan planlanmış fazla mesai süresi miktarı."
type: docs
weight: 980
url: /tr/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

Kalan planlanmış fazla mesai süresi miktarı.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## Örnekler

Tsk.RemainingOvertimeWork özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


