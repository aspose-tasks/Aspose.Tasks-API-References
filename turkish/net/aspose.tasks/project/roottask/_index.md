---
title: "Project.RootTask"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Görevlerin ağacının kökünü alır."
type: docs
weight: 800
url: /tr/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

Görev ağacının kökünü alır.

```csharp
public Task RootTask { get; }
```

## Örnekler

Kök proje görevini kullanarak bir projeye görev eklemenin nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


