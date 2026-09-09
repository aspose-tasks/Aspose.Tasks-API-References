---
title: "Project.Get"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Bu konteynerde özelliğin eşlendiği değeri döndürür"
type: docs
weight: 1080
url: /tr/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

Bu kapsayıcıda özelliğin eşlendiği değeri döndürür.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| Parametre | Açıklama |
| --- | --- |
| T | eşlenen değerin tipi. |
| key | belirtilen özellik anahtarı. Özellik anahtarını almak için [`Prj`](../../prj/). |

### Dönüş Değeri

özelliğin bu konteynerde eşlendiği değer.

## Örnekler

Bir proje sürümünün nasıl kontrol edileceğini gösterir.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Proje sürümünü göster
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


