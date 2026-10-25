---
title: "Yapı KeyTK"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Key2TK yapısı. Belirtilen türde bir sınıfın özellik anahtarını temsil eder. Bu sınıfın bir örneği, bir kapsayıcının özelliğini alırken veya ayarlarken kullanılır."
type: docs
weight: 930
url: /tr/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

Belirtilen türde bir sınıfın özellik anahtarını temsil eder. Bu sınıfın bir örneği, bir kapsayıcının özelliğini alırken veya ayarlarken kullanılır.

```csharp
public struct Key<T, K>
    where K : struct
```

| Parametre | Açıklama |
| --- | --- |
| T | Özellik değerinin türü. |
| K | Özellik anahtarının türü. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | Özelliğin anahtarını alır. |

## Örnekler

Prj.ActualsInSync özelliğini okuma/yazma işleminin nasıl yapılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


