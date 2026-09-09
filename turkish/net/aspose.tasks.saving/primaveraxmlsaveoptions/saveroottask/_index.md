---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraXmlSaveOptions özelliği. Kök görevinin kaydedilip kaydedilmeyeceğini belirten bir değeri alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

Kök görevin kaydedilip kaydedilmeyeceğini gösteren bir değeri alır veya ayarlar.

```csharp
public bool SaveRootTask { get; set; }
```

## Örnekler

Primavera XML dosyasına nasıl dışa aktarılacağını gösterir.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Ayrıca Bakınız

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


