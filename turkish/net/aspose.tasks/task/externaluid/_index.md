---
title: "Task.ExternalUid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Görev dışarıdan olduğunda dış görevlerin benzersiz tanımlayıcısını alır veya ayarlar"
type: docs
weight: 430
url: /tr/net/aspose.tasks/task/externaluid/
---
## Task.ExternalUid property

Görev dışsal olduğunda dış görevin Benzersiz tanımlayıcısını alır veya ayarlar.

```csharp
public int ExternalUid { get; set; }
```

## Örnekler

Çapraz proje görev bağlantısı oluşturmayı gösterir - başka bir (dış) projedeki göreve bağlantı.

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// Başka bir projedeki göreve bir bağlantı oluşturmak için şunu yaratmalıyız
// geçerli projede onun kopyasını (veya "dış") görevi.

Task t2 = summary.Children.Add("External Task");
t2.Set(Tsk.ExternalTaskProject, "ExternalProject.mpp"); // here we set path to external project's MPP file.
t2.Set(Tsk.ExternalId, 1); // Set External task's Id.
t2.Set(Tsk.ExternalUid, 2); // External task's Unique Id should be set.
t2.Set(Tsk.IsExternalTask, true);
t2.Set(Tsk.IsManual, new NullableBool(false));
t2.Set(Tsk.IsSummary, false);

Task t = summary.Children.Add("Task");
TaskLink link = project.TaskLinks.Add(t2, t);
link.IsCrossProject = true;
link.LinkType = TaskLinkType.FinishToStart;
link.CrossProjectName = "ExternalProject.mpp\\\\1"; // <- here external task's Id is used.
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


