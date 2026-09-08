---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PrimaveraXmlSaveOptions. Obtiene o establece un valor que indica si se debe guardar una tarea raíz o no"
type: docs
weight: 20
url: /es/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

Obtiene o establece un valor que indica si guardar una tarea raíz o no.

```csharp
public bool SaveRootTask { get; set; }
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


