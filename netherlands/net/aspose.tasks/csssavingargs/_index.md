---
title: "Klasse CssSavingArgs"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CssSavingArgs klasse. Deze klasse vertegenwoordigt een set gegevens die gerelateerd zijn aan het opslaan van externe CSS-bestanden dat plaatsvindt tijdens de conversie naar HTML-indeling."
type: docs
weight: 360
url: /nl/net/aspose.tasks/csssavingargs/
---
## CssSavingArgs class

Deze klasse stelt een set gegevens voor die gerelateerd zijn aan het opslaan van een extern CSS‑bestand dat optreedt tijdens de conversie naar HTML‑formaat.

```csharp
public class CssSavingArgs : ResourceSavingArgs
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [CssSavingArgs](csssavingargs/)() | Initialiseert een nieuw exemplaar van de `CssSavingArgs`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [FileName](../../aspose.tasks/resourcesavingargs/filename/) { get; set; } | Haalt op of stelt de veronderstelde bestandsnaam in die van de converter naar de code van een aangepaste methode gaat. Kan worden gebruikt in aangepaste code om te bepalen hoe het bestand moet worden verwerkt of waar het moet worden opgeslagen. |
| [KeepStreamOpen](../../aspose.tasks/resourcesavingargs/keepstreamopen/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de stream open blijft nadat het opslaan van de bron is voltooid. |
| [Stream](../../aspose.tasks/resourcesavingargs/stream/) { get; set; } | Haalt op of stelt de binaire inhoud van het opgeslagen bestand in. |
| [Uri](../../aspose.tasks/resourcesavingargs/uri/) { get; set; } | Haalt op of stelt de resource‑URI in. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CloseStreamIfRequired](../../aspose.tasks/resourcesavingargs/closestreamifrequired/)() | Sluit de stream als KeepStreamOpen onwaar is, anders spoelt u deze. |

## Voorbeelden

Toont hoe CSS-opslagargumenten gespecificeerd worden.

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

### Zie ook

* class [ResourceSavingArgs](../resourcesavingargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


