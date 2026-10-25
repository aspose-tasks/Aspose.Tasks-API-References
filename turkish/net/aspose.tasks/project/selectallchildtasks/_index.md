---
title: "Project.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Kök görevinin tüm alt görevlerini özyinelemeli olarak toplar"
type: docs
weight: 1230
url: /tr/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

Kök görevin tüm alt görevlerini özyinelemeli olarak toplar.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Dönüş Değeri

Görevlerin koleksiyonu.

## Örnekler

Seçili görevlerin WBS kodlarını yeniden numaralandırmanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// çıktı: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// çıktı: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Ayrıca Bakınız

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


