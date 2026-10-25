---
title: "Sınıf TaskLinkCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskLinkCollection sınıfı. Task nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 2420
url: /tr/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

[`Task`](../task/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | `TaskLinkCollection` nesnesinde bulunan nesne sayısını alır. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür veya ayarlar. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | ResourceAssignmentCollection nesnesinin üst proje nesnesini alır. Bu nesne için üst [`Project`](../project/) nesnesi. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | Bu, ICollection'ın Add metodunun sadece NotSupportedException fırlatan taslak uygulamasıdır |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | TaskLinkCollection nesnesine eklenmiş Finish-Start [`TaskLink`](../tasklink/) örneğini döndürür. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | TaskLinkCollection nesnesine eklenmiş [`TaskLink`](../tasklink/) örneğini döndürür. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | TaskLinkCollection nesnesine eklenmiş [`TaskLink`](../tasklink/) örneğini döndürür. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | Bir projeden görev bağlantısını kaldırır. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | TaskLinkCollection nesnesini [`TaskLink`](../tasklink/) nesnelerinin bir listesine dönüştürür. |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


