---
title: "Tsk.IsResumeValid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin devam ettirilebilip getirilemeyeceğini belirler"
type: docs
weight: 680
url: /tr/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

Bir görevin yeniden başlatılıp başlatılamayacağını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## Örnekler

Tsk.IsResumeValid özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


