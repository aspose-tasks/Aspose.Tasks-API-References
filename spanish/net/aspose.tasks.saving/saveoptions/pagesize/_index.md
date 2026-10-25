---
title: "SaveOptions.PageSize"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece el tamaño de página a renderizar. El valor predeterminado es PageSize.A4"
type: docs
weight: 130
url: /es/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

Obtiene o establece el tamaño de la página a renderizar (El valor predeterminado es PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## Ejemplos

Muestra cómo establecer el tamaño de página (puede ser uno de los valores de la enumeración &lt;see cref=\"P:Aspose.Tasks.Visualization.TiffCompression\" /&gt;).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// Renderiza el proyecto a todos los tamaños de página predefinidos
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### Ver también

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


