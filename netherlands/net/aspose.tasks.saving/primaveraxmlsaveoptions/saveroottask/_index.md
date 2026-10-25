---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraXmlSaveOptions eigenschap. Haalt een waarde op of stelt deze in die aangeeft of een hoofdtaak al dan niet moet worden opgeslagen"
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

Haalt een waarde op of stelt deze in die aangeeft of een hoofdtaak moet worden opgeslagen of niet.

```csharp
public bool SaveRootTask { get; set; }
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


