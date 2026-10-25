---
title: "SaveOptions.IsPortrait"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal."
type: docs
weight: 70
url: /es/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Obtiene o establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.

```csharp
public bool IsPortrait { get; set; }
```

## Observaciones

No es aplicable cuando SaveOptions.PageSize == Visualization.PageSize.DefinedInView. En este caso se usa View.PageInfo.PageSettings.IsPortrait. No es aplicable cuando SaveOptions.CustomPageSize está configurado.

## Ejemplos

Muestra cómo especificar el tamaño y la orientación de la página usando la configuración View o usando SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// En este caso, el tamaño y la orientación de la página se aplican a partir de las propiedades view.PageInfo.PageSettings.PaperSize y view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// En este caso, el tamaño y la orientación de la página se aplican a partir de las propiedades de SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// En este caso, el tamaño de la página se aplica a partir de SaveOptions.CustomPageSize. La propiedad IsPortrait no se tiene en cuenta.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


