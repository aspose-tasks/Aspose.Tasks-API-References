---
title: "LoadOptions.CancellationToken"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "LoadOptions özelliği. Bir proje yükleme işlemini iptal etmek için kullanılabilecek bir token alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

Proje yükleme işlemini iptal etmek için kullanılabilecek bir token alır veya ayarlar.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Örnekler

Uzun süren bir Proje yükleme işlemini iptal etmek için CancellationToken'ın nasıl geçirileceğini gösterir.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts, proje yükleme işlemini iptal etmek için cts.Cancel() metodunun çağrılabileceği başka bir iş parçacığına geçirilebilir.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


