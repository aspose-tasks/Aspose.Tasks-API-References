---
title: "Tsk.DisplayOnTimeline"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin zaman çizelgesi görünümünde gösterilip gösterilmeyeceğini belirtir"
type: docs
weight: 290
url: /tr/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

Bir görevin zaman çizelgesi görünümünde gösterilip gösterilmeyeceğini belirtir.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## Örnekler

Tsk.DisplayOnTimeline özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


