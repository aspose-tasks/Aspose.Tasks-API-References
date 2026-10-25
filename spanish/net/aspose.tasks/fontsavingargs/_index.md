---
title: "Clase FontSavingArgs"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.FontSavingArgs. Esta clase representa un conjunto de datos relacionados con el guardado de archivos de fuentes externas que ocurre durante la conversión al formato HTML."
type: docs
weight: 680
url: /es/net/aspose.tasks/fontsavingargs/
---
## FontSavingArgs class

Esta clase representa un conjunto de datos relacionados con el guardado de archivos de fuentes externas que ocurre durante la conversión al formato HTML.

```csharp
public class FontSavingArgs : ResourceSavingArgs
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FontSavingArgs](fontsavingargs/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FileName](../../aspose.tasks/resourcesavingargs/filename/) { get; set; } | Obtiene o establece el nombre de archivo supuesto que pasa del convertidor al código del método personalizado. Puede usarse en código personalizado para decidir cómo procesar o dónde guardar ese archivo. |
| [KeepStreamOpen](../../aspose.tasks/resourcesavingargs/keepstreamopen/) { get; set; } | Obtiene o establece un valor que indica si el flujo permanecerá abierto después de que finalice el guardado del recurso. |
| [Stream](../../aspose.tasks/resourcesavingargs/stream/) { get; set; } | Obtiene o establece el contenido binario del archivo guardado. |
| [Uri](../../aspose.tasks/resourcesavingargs/uri/) { get; set; } | Obtiene o establece el URI del recurso. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CloseStreamIfRequired](../../aspose.tasks/resourcesavingargs/closestreamifrequired/)() | Cierra el flujo si KeepStreamOpen es false, de lo contrario vacíalo. |

## Ejemplos

Muestra cómo trabajar con los argumentos de guardado de fuentes.

```csharp
public void ResourcePrefixForNestedResourcesExample()
{
    var project = new Project(DataDir + "Project1.mpp");
    var options = ResourcePrefixForNestedResources.GetSaveOptions(1);
    project.Save(OutDir + "document_out.html", options);
}

private class ResourcePrefixForNestedResources : ICssSavingCallback, IFontSavingCallback, IImageSavingCallback
{
    public void CssSaving(CssSavingArgs args)
    {
        if (!Directory.Exists(OutDir + "css/"))
        {
            Directory.CreateDirectory(OutDir + "css/");
        }

        var stream = new FileStream(OutDir + "css/" + args.FileName, FileMode.Create);
        args.Stream = stream;
        args.KeepStreamOpen = false;
        args.Uri = OutDir + "css/" + args.FileName;
    }

    public void FontSaving(FontSavingArgs args)
    {
        if (!Directory.Exists(OutDir + "fonts/"))
        {
            Directory.CreateDirectory(OutDir + "fonts/");
        }

        var stream = new FileStream(OutDir + "fonts/" + args.FileName, FileMode.Create);
        args.Stream = stream;
        args.KeepStreamOpen = false;
        args.Uri = OutDir + "fonts/" + args.FileName;
    }

    public void ImageSaving(ImageSavingArgs args)
    {
        if (!Directory.Exists(OutDir + "resources/"))
        {
            Directory.CreateDirectory(OutDir + "resources/");
        }

        if (!Directory.Exists(OutDir + "resources/nestedResources/"))
        {
            Directory.CreateDirectory(OutDir + "resources/nestedResources/");
        }

        if (args.FileName.EndsWith("png"))
        {
            var stream1 = new FileStream(OutDir + "resources/nestedResources/" + args.FileName, FileMode.Create);
            args.Stream = stream1;
            args.KeepStreamOpen = false;
            args.Uri = OutDir + "resources/" + args.FileName;

            // args.NestedUri = dataDir + \"nestedResources/\" + args.FileName;
        }
        else
        {
            var stream2 = new FileStream(OutDir + "resources/" + args.FileName, FileMode.Create);
            args.Stream = stream2;
            args.KeepStreamOpen = false;
            args.Uri = OutDir + "resources/" + args.FileName;
        }
    }

    public static HtmlSaveOptions GetSaveOptions(int pageNumber)
    {
        var options = new HtmlSaveOptions
                          {
                              Pages = new List<int>(),
                              IncludeProjectNameInPageHeader = false,
                              IncludeProjectNameInTitle = false,
                              PageSize = PageSize.A3,
                              Timescale = Timescale.ThirdsOfMonths,
                              ReduceFooterGap = true,
                              FontFaceTypes = FontFaceType.Ttf,
                              ExportCss = ResourceExportType.AsFile,
                              ExportFonts = ResourceExportType.AsFile,
                              ExportImages = ResourceExportType.AsFile
                          };

        var program = new ResourcePrefixForNestedResources();
        options.FontSavingCallback = program;
        options.CssSavingCallback = program;
        options.ImageSavingCallback = program;

        options.Pages.Clear();
        options.Pages.Add(pageNumber);

        if (!Directory.Exists(DataDir + "fonts"))
        {
            Directory.CreateDirectory(DataDir + "fonts");
        }

        if (!Directory.Exists(DataDir + "resources"))
        {
            Directory.CreateDirectory(DataDir + "resources");
        }

        if (!Directory.Exists(DataDir + "nestedResources"))
        {
            Directory.CreateDirectory(DataDir + "resources/nestedResources");
        }

        if (!Directory.Exists(DataDir + "css"))
        {
            Directory.CreateDirectory(DataDir + "css");
        }

        return options;
    }
}
```

### Ver también

* class [ResourceSavingArgs](../resourcesavingargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


