---
title: "SaveOptions.ViewSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece una vista View para renderizar. Puede usar esta opción para especificar explícitamente qué vista debe guardarse en formatos PDF, HTML o Image. Si esta propiedad está establecida, la propiedad PresentationFormat se ignora cuando se guarda el proyecto. La vista debe ser una de las siguientes pantallas Screen: Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage."
type: docs
weight: 240
url: /es/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Obtiene o establece una vista ([`View`](../view/)) para renderizar. Puede usar esta opción para especificar explícitamente qué vista debe guardarse en formatos PDF, HTML o Image. Si esta propiedad está establecida, la propiedad [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) se ignora cuando se guarda el proyecto. La vista debe ser una de las siguientes pantallas (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

```csharp
public View ViewSettings { get; set; }
```

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Cuando se llama al método set y se proporciona una instancia de la clase View con un valor no compatible de la propiedad Screen. |

## Ejemplos

Muestra cómo usar 'SaveOptions.ViewSettings' para especificar la vista que debe renderizarse a PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### Ver también

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


