---
title: "Task.SplitParts"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Bir görevin bölümlerini temsil eden bir SplitPart koleksiyonu alır"
type: docs
weight: 1110
url: /tr/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

Bir görevin bölümlerini temsil eden SplitPart koleksiyonunu alır.

```csharp
public SplitPartCollection SplitParts { get; }
```

## Örnekler

Görevin bölünmüş parçalarının nasıl görüntüleneceğini gösterir.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// Göreve eriş 
var task = project.RootTask.Children.GetById(4);

// Görevin bölünmüş parçalarını görüntüle
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### Ayrıca Bakınız

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


