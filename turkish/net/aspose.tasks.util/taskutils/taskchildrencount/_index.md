---
title: "TaskUtils.TaskChildrenCount"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskUtils yöntemi. Tüm seviyelerde görevlerin alt görev sayısını yinelemeli olarak hesaplar"
type: docs
weight: 40
url: /tr/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

Tüm seviyelerde görevlerin alt görev sayısını özyinelemeli olarak hesaplar.

```csharp
public static int TaskChildrenCount(Task task)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | Görev | Alt görevleri hesaplanan görev. |

### Dönüş Değeri

Alt görev sayısı.

## Örnekler

Nasıl kullanılacağını gösterir &lt;see cref="Aspose.Tasks.Util.TaskUtils.TaskChildrenCount" /&gt; yöntemi.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Tüm seviyelerde görevlerin alt görev sayısını yinelemeli olarak hesaplar
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### Ayrıca Bakınız

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


