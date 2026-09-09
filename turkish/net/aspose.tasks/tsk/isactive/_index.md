---
title: "Tsk.IsActive"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk field. Bir görevin aktif olup olmadığını belirler. Pasif görevler artık diğer görevleri veya genel Proje takvimini etkilemez"
type: docs
weight: 550
url: /tr/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

Bir görevin aktif olup olmadığını belirler. Pasif görevler artık diğer görevleri veya genel Proje zamanlamasını etkilemez.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## Örnekler

Tsk.IsActive özelliğini okuma/yazma nasıl gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


