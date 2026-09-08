---
title: "ImageSaveOptions.Pages"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ImageSaveOptions. Obtiene o establece una lista de números de página para guardar al exportar el diseño del proyecto a archivos separados. Todas las páginas se guardarán si esta lista está vacía."
type: docs
weight: 50
url: /es/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

Obtiene o establece una lista de números de página a guardar al guardar el diseño del proyecto en archivos separados. Todas las páginas se guardarán si esta lista está vacía.

```csharp
public List<int> Pages { get; set; }
```

## Ejemplos

Muestra cómo guardar páginas seleccionadas como una imagen.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### Ver también

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


