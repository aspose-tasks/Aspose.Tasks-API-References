---
title: "Tsk.IsPublished"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Mevcut görevin, projenin geri kalanıyla birlikte Project Server'a yayınlanıp yayınlanmayacağını belirler"
type: docs
weight: 660
url: /tr/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

Mevcut görevin, projenin geri kalanıyla birlikte Project Server'a yayınlanıp yayınlanmayacağını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## Örnekler

Tsk.IsPublished özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


