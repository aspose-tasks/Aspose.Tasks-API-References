---
title: "Project.RenumberWBSCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Tüm görevlerin WBS kodunu yeniden numaralandırır"
type: docs
weight: 1180
url: /tr/net/aspose.tasks/project/renumberwbscode/
---
## RenumberWBSCode() {#renumberwbscode}

Tüm görevlerin WBS kodunu yeniden numaralandırır.

```csharp
public void RenumberWBSCode()
```

## Örnekler

Görevlerin WBS kodlarını yeniden numaralandırmanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

IEnumerable<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// çıktı: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode();

Console.WriteLine("\nWBS codes after: ");

// çıktı: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RenumberWBSCode(List&lt;int&gt;) {#renumberwbscode_1}

Geçmiş görevlerin WBS kodunu yeniden numaralandırır.

```csharp
public void RenumberWBSCode(List<int> taskIds)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| taskIds | List`1 | WBS kodlarını yeniden numaralandırmak için görev tanımlayıcıları. |

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

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


