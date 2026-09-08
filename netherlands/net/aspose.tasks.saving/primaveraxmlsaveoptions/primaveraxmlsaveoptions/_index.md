---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraXmlSaveOptions constructor. Initialiseert een nieuw exemplaar van de PrimaveraXmlSaveOptions-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

Initialiseert een nieuw exemplaar van de [`PrimaveraXmlSaveOptions`](../) klasse.

```csharp
public PrimaveraXmlSaveOptions()
```

## Voorbeelden

Toont hoe te exporteren naar een Primavera‑XML‑bestand.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Zie ook

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


