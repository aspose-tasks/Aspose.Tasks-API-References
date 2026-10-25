---
title: "Task.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Bu Task için bir hash kodu değeri döndürür."
type: docs
weight: 1350
url: /tr/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

Bu Görev için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

bu nesne için bir karma kod değeri döndürür.

## Örnekler

Bir görevin hash kodunun nasıl alınacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// bir görevin karma kodu, görevin uid'si ve adına dayanır
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


