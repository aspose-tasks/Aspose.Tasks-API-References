---
title: "Sınıf CopyToOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CopyToOptions sınıfı. Proje verileri kopyalanırken ek seçenekler belirtmeye olanak tanır"
type: docs
weight: 340
url: /tr/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

Proje verilerini kopyalarken ek seçenekleri belirtmeye olanak tanır.

```csharp
public class CopyToOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CopyToOptions](copytooptions/)() | `CopyToOptions` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | Proje verileri kopyalanırken görünüm verilerinin kopyalanıp kopyalanmayacağını gösteren bir değeri alır veya ayarlar. Varsayılan değer true. |

## Örnekler

Proje kopyalama seçeneklerinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// Ortak proje verileri kopyalanırken görünüm verilerinin kopyalanmasını atla.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


