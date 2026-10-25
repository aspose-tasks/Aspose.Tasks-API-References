---
title: "Tsk.HideBar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Microsoft Project'te gösterildiğinde bir görevin Gantt çubuğunun gizlenip gizlenmeyeceğini belirler."
type: docs
weight: 480
url: /tr/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Microsoft Project'te görüntülendiğinde bir görevin Gantt çubuğunun gizli olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## Örnekler

Tsk.HideBar özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


