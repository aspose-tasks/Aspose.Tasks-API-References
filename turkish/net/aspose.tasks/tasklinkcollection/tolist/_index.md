---
title: "TaskLinkCollection.ToList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLinkCollection yöntemi. TaskLinkCollection nesnesini TaskLink nesnelerinin bir listesine dönüştürür"
type: docs
weight: 70
url: /tr/net/aspose.tasks/tasklinkcollection/tolist/
---
## TaskLinkCollection.ToList method

TaskLinkCollection nesnesini [`TaskLink`](../../tasklink/) nesnelerinin bir listesine dönüştürür.

```csharp
public List<TaskLink> ToList()
```

### Dönüş Değeri

[`TaskLink`](../../tasklink/) nesnelerinin listesi.

## Örnekler

Görev bağlantısı koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// görevleri al
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// görevleri bağla
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// görevler arasındaki bağlantıları yazdır
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// indeks erişimiyle bağlantıyı düzenle
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// tüm görev bağlantılarını kaldır
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Ayrıca Bakınız

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


