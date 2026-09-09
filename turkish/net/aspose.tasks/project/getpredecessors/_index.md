---
title: "Project.GetPredecessors"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Belirtilen görevin öncülleri olan görev bağlantılarının bir koleksiyonunu döndürür."
type: docs
weight: 1120
url: /tr/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

Belirtilen görevin öncülleri olan görev bağlantılarının bir koleksiyonunu döndürür.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | Görev | Öncülleri alınacak görev. |

### Dönüş Değeri

Öncüllerin listesi [`TaskLink`](../../tasklink/).

## Örnekler

Belirli bir görev için öncüllerin nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// Öncül ve sonraki görevlerin adlarını göster
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### Ayrıca Bakınız

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


