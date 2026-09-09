---
title: "CopyToOptions.CopyToOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CopyToOptions yapıcı. CopyToOptions sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

[`CopyToOptions`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public CopyToOptions()
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


