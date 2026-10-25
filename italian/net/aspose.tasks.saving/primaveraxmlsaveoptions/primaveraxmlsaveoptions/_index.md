---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore PrimaveraXmlSaveOptions. Inizializza una nuova istanza della classe PrimaveraXmlSaveOptions"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

Inizializza una nuova istanza della classe [`PrimaveraXmlSaveOptions`](../).

```csharp
public PrimaveraXmlSaveOptions()
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


