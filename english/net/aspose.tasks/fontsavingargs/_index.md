---
title: Class FontSavingArgs
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.FontSavingArgs class. This class represents set of data that related to external fonts files saving that occurs during conversion to HTML format
type: docs
weight: 680
url: /net/aspose.tasks/fontsavingargs/
---
## FontSavingArgs class

This class represents set of data that related to external fonts file's saving that occurs during conversion to HTML format.

```csharp
public class FontSavingArgs : ResourceSavingArgs
```

## Constructors

| Name | Description |
| --- | --- |
| [FontSavingArgs](fontsavingargs/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [FileName](../../aspose.tasks/resourcesavingargs/filename/) { get; set; } | Gets or sets the supposed file name that goes from converter to code of custom method. Can be use in custom code to decide how to process or where save that file. |
| [KeepStreamOpen](../../aspose.tasks/resourcesavingargs/keepstreamopen/) { get; set; } | Gets or sets a value indicating whether the stream will be kept open after resource saving finishes. |
| [Stream](../../aspose.tasks/resourcesavingargs/stream/) { get; set; } | Gets or sets the binary content of saved file. |
| [Uri](../../aspose.tasks/resourcesavingargs/uri/) { get; set; } | Gets or sets the resource URI. |

## Methods

| Name | Description |
| --- | --- |
| [CloseStreamIfRequired](../../aspose.tasks/resourcesavingargs/closestreamifrequired/)() | Close stream if KeepStreamOpen is false, else flush it. |

## Examples

Shows how to work with font saving args.

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

            // args.NestedUri = dataDir + "nestedResources/" + args.FileName;
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

### See Also

* class [ResourceSavingArgs](../resourcesavingargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


