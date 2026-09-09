---
title: "CopyToOptions.CopyViewData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CopyToOptions özelliği. Proje verileri kopyalanırken görünüm verilerinin kopyalanıp kopyalanmayacağını belirten bir değeri alır veya ayarlar. Varsayılan değer true'tur."
type: docs
weight: 20
url: /tr/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

Proje verileri kopyalanırken görünüm verilerinin kopyalanıp kopyalanmayacağını gösteren bir değeri alır veya ayarlar. Varsayılan değer true.

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


