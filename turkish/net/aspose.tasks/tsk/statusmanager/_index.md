---
title: "Tsk.StatusManager"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Kaynaklardan mevcut görev için durum güncellemelerini alacak kurumsal kaynağın adı"
type: docs
weight: 1050
url: /tr/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

Kaynaklardan mevcut görev için durum güncellemelerini alacak kurumsal kaynağın adı.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## Örnekler

Tsk.StatusManager özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


