---
title: "TaskLinkCollection.Add"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLinkCollection yöntemi. TaskLinkCollection nesnesine eklenen FinishStart TaskLink örneğini döndürür."
type: docs
weight: 40
url: /tr/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Finish-Start [`TaskLink`](../../tasklink/) örneğini döndürür; bu örnek TaskLinkCollection nesnesine eklenmiştir.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pred | Görev | Önceki görev. |
| succ | Görev | Sonraki görev. |

### Dönüş Değeri

Bu nesneye eklenmiş bir görev bağlantısı örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | Girdi görevlerinden herhangi biri null ise ArgumentNullException fırlatılacaktır. |

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
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

`[`TaskLink`](../../tasklink/)` örneğini döndürür; bu örnek TaskLinkCollection nesnesine eklenmiştir.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pred | Görev | Önceki görev. |
| succ | Görev | Sonraki görev. |
| linkType | TaskLinkType | Bağlantı türü [`TaskLinkType`](../../tasklinktype/) |

### Dönüş Değeri

Bu nesneye eklenmiş bir görev bağlantısı örneği.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | Girdi görevlerinden herhangi biri null ise ArgumentNullException fırlatılacaktır. |

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
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

`[`TaskLink`](../../tasklink/)` örneğini döndürür; bu örnek TaskLinkCollection nesnesine eklenmiştir.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pred | Görev | Önceki görev. |
| succ | Görev | Sonraki görev. |
| linkType | TaskLinkType | Bağlantı türü [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Bağlantı gecikmesi [`Duration`](../../duration/). |

### Dönüş Değeri

Bu nesneye eklenmiş bir görev bağlantısı.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | Girdi görevlerinden herhangi biri null ise ArgumentNullException fırlatılacaktır. |

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
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Bu, ICollection'ın Add metodunun sadece NotSupportedException fırlatan taslak uygulamasıdır

```csharp
public void Add(TaskLink item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | TaskLink | Eklenecek öğe. |

### Ayrıca Bakınız

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


