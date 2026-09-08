---
title: "XpsOptions.XpsOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de XpsOptions. Inicializa una nueva instancia de la clase XpsOptions"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

Inicializa una nueva instancia de la clase [`XpsOptions`](../).

```csharp
public XpsOptions()
```

## Ejemplos

Muestra cómo guardar el proyecto como archivo XPS.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// crear opciones de guardado XPS y ajustar los parámetros
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### Ver también

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


