---
title: "TaskLink.CrossProjectName"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLink özelliği. Dış öncül projeyi alır veya ayarlar"
type: docs
weight: 10
url: /tr/net/aspose.tasks/tasklink/crossprojectname/
---
## TaskLink.CrossProjectName property

Harici öncül projeyi alır veya ayarlar.

```csharp
public string CrossProjectName { get; set; }
```

## Örnekler

Çapraz proje görev bağlantılarını nasıl bulacağını gösterir.

```csharp
var project = new Project(DataDir + "GetCrossProjectTaskLinks.mpp");

// Çapraz proje görev bağlantılarını kontrol et
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Task Link: " + taskLink.ToString());
    if (taskLink.IsCrossProject)
    {
        Console.WriteLine(taskLink.CrossProjectName);
    }
}
```

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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


