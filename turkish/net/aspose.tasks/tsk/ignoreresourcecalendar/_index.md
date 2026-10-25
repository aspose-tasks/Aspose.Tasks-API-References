---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevin zamanlamasının, göreve atanan kaynakların takvimlerini dikkate alıp almayacağını belirler"
type: docs
weight: 530
url: /tr/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

Görevin zamanlamasının, göreve atanmış kaynakların takvimlerini dikkate alıp almadığını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## Örnekler

Tsk.IgnoreResourceCalendar özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


