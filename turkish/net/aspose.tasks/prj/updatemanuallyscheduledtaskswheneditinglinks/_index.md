---
title: "Prj.UpdateManuallyScheduledTasksWhenEditingLinks"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bağlantılar düzenlendiğinde manuel görevlerin güncellenip güncellenmeyeceğini belirler"
type: docs
weight: 770
url: /tr/net/aspose.tasks/prj/updatemanuallyscheduledtaskswheneditinglinks/
---
## Prj.UpdateManuallyScheduledTasksWhenEditingLinks field

Bağlantılar düzenlendiğinde manuel görevlerin güncellenmesi gerekip gerekmediğini belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> UpdateManuallyScheduledTasksWhenEditingLinks;
```

## Örnekler

Prj.UpdateManuallyScheduledTasksWhenEditingLinks özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.UpdateManuallyScheduledTasksWhenEditingLinks, true);

Console.WriteLine("Update Manually Scheduled Tasks When Editing Links: " + project.Get(Prj.UpdateManuallyScheduledTasksWhenEditingLinks));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


