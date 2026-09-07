---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor PrimaveraXmlSaveOptions. Menginisialisasi instance baru dari kelas PrimaveraXmlSaveOptions"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

Menginisialisasi instance baru dari kelas [`PrimaveraXmlSaveOptions`](../).

```csharp
public PrimaveraXmlSaveOptions()
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


