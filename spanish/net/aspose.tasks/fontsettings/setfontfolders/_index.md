---
title: "FontSettings.SetFontFolders"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método FontSettings. Establece las carpetas donde Aspose.Tasks busca fuentes TrueType al renderizar la vista de proyectos"
type: docs
weight: 50
url: /es/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Establece las carpetas donde Aspose.Tasks busca fuentes TrueType al renderizar la vista del proyecto.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolders | String[] | Una matriz de carpetas que contienen fuentes TrueType. |
| recursive | Boolean | Si es true, las carpetas especificadas se escanearán de forma recursiva. |

## Ejemplos

Muestra cómo establecer una carpeta de fuentes personalizada.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// Los archivos de fuentes TrueType para todas las fuentes usadas en el proyecto abierto deben estar ubicados en la carpeta MyFonts.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### Ver también

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


