---
title: "Tsk.ActualWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevlere atanan kaynaklar tarafından zaten yapılan iş miktarı"
type: docs
weight: 90
url: /tr/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

Görevlere atanan kaynaklar tarafından zaten yapılan iş miktarı.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## Örnekler

Tsk.ActualWork özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


