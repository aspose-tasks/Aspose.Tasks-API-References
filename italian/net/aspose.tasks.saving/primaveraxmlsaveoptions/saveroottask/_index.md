---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PrimaveraXmlSaveOptions. Ottiene o imposta un valore che indica se salvare o meno un'attività radice"
type: docs
weight: 20
url: /it/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

Ottiene o imposta un valore che indica se salvare o meno un'attività radice.

```csharp
public bool SaveRootTask { get; set; }
```

## Esempi

Mostra come esportare il file in XML Primavera.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Vedi anche

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


