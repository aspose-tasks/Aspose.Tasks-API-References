---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraXmlSaveOptions yapıcı. PrimaveraXmlSaveOptions sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

[`PrimaveraXmlSaveOptions`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public PrimaveraXmlSaveOptions()
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


