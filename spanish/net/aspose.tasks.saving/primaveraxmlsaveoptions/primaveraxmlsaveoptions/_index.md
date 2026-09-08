---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de PrimaveraXmlSaveOptions. Inicializa una nueva instancia de la clase PrimaveraXmlSaveOptions"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

Inicializa una nueva instancia de la clase [`PrimaveraXmlSaveOptions`](../).

```csharp
public PrimaveraXmlSaveOptions()
```

## Ejemplos

Muestra cómo exportar al archivo XML de Primavera.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Ver también

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


