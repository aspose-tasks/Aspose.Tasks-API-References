---
title: "Task.Clone"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Alt görevler olmadan bir görevin tam bir kopyasını oluşturur"
type: docs
weight: 1310
url: /tr/net/aspose.tasks/task/clone/
---
## Task.Clone method

Alt görevler olmadan bir görevin tam bir kopyasını oluşturur.

```csharp
public object Clone()
```

### Dönüş Değeri

Bir görevin kopyası oluşturuldu.

## Örnekler

Bir görevi nasıl klonlayacağınızı gösterir.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


