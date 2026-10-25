---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad XpsOptions. Obtiene o establece un valor que indica si un metafile debe renderizarse como bitmap."
type: docs
weight: 20
url: /es/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

Obtiene o establece un valor que indica si un metafile debe renderizarse como bitmap.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
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


