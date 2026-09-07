---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PrimaveraXmlSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menyimpan tugas root atau tidak"
type: docs
weight: 20
url: /id/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

Mendapatkan atau mengatur nilai yang menunjukkan apakah menyimpan tugas root atau tidak.

```csharp
public bool SaveRootTask { get; set; }
```

## Contoh

Menampilkan cara mengekspor ke file Primavera XML.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Lihat Juga

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


