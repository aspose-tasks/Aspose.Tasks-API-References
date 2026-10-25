---
title: "Project.CriticalPath"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Bu projenin Kritik Yolunu oluşturan Kritik görevlerin bir listesini içeren bir koleksiyon alır. Bu, n'in projedeki görev sayısı olduğu bir On işlemidir."
type: docs
weight: 180
url: /tr/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

Bu projenin Kritik Yolunu oluşturan Kritik görevlerin bir listesini içeren bir koleksiyonu alır. Bu, projedeki görev sayısı n olduğunda O(n) bir işlemdir.

```csharp
public TaskCollection CriticalPath { get; }
```

### Dönüş Değeri

tüm kritik görevlerin bir listesini temsil eden bir koleksiyon.

## Örnekler

Projenin kritik yolunu nasıl hesaplayacağını gösterir.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// Kritik yolu şimdi göster
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### Ayrıca Bakınız

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


