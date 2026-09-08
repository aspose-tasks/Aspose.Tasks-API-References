---
title: "PageViewSettings.PrintNotes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageViewSettings. Obtiene o establece un valor que indica si se imprimen notas"
type: docs
weight: 70
url: /es/net/aspose.tasks.visualization/pageviewsettings/printnotes/
---
## PageViewSettings.PrintNotes property

Obtiene o establece un valor que indica si se imprimen notas.

```csharp
public bool PrintNotes { get; set; }
```

## Ejemplos

Muestra cómo imprimir notas de tareas, recursos y asignaciones en una página separada.

```csharp
var project = new Project(DataDir + "Input.mpp");

// establece el número de primeras columnas que se imprimirán en todas las páginas
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// establece un valor que indica si se imprimen notas.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// establece un valor que indica si se ajusta la escala de tiempo al final de una página al imprimir.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// establece un valor que indica si se imprimen todas las columnas de hoja de una vista
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// establece un valor que indica si se imprimen páginas en blanco de una vista
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// establece un valor que indica si se deben imprimir un número especificado de primeras columnas en todas las páginas
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### Ver también

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


