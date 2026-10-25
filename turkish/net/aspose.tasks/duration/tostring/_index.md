---
title: "Duration.ToString"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration yöntemi. Bu örneğin string temsili döndürür"
type: docs
weight: 120
url: /tr/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

Bu örneğin dize temsili döndürür.

```csharp
public override string ToString()
```

### Dönüş Değeri

Bu örneğin string temsili.

## Örnekler

Bir süreyi stringe nasıl dönüştüreceğinizi gösterir.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// görev süresini al
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### Ayrıca Bakınız

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


