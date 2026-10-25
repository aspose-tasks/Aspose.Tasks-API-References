---
title: "Task.Children"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Bu nesnenin bir alt görev koleksiyonunu alır. Çocuk görevleri temsil eden TaskCollection nesnesi"
type: docs
weight: 190
url: /tr/net/aspose.tasks/task/children/
---
## Task.Children property

Bu nesnenin alt görev koleksiyonunu alır. Çocuk görevleri temsil eden TaskCollection nesnesi.

```csharp
public TaskCollection Children { get; }
```

## Örnekler

Bir görev eklemek için görev koleksiyonunun nasıl kullanılacağını gösterir.

```csharp
var project = new Project();

// Görev, alt görev ekle ve projeyi kaydet
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


