---
title: "Κλάση FontSavingArgs"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.FontSavingArgs κλάση. Αυτή η κλάση αντιπροσωπεύει ένα σύνολο δεδομένων που σχετίζονται με την αποθήκευση εξωτερικών αρχείων γραμματοσειρών που συμβαίνει κατά τη μετατροπή σε μορφή HTML."
type: docs
weight: 680
url: /el/net/aspose.tasks/fontsavingargs/
---
## FontSavingArgs class

Αυτή η κλάση αντιπροσωπεύει ένα σύνολο δεδομένων που σχετίζονται με την αποθήκευση εξωτερικού αρχείου γραμματοσειρών που συμβαίνει κατά τη μετατροπή σε μορφή HTML.

```csharp
public class FontSavingArgs : ResourceSavingArgs
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [FontSavingArgs](fontsavingargs/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [FileName](../../aspose.tasks/resourcesavingargs/filename/) { get; set; } | Λαμβάνει ή ορίζει το υποτιθέμενο όνομα αρχείου που περνά από τον μετατροπέα στον κώδικα της προσαρμοσμένης μεθόδου. Μπορεί να χρησιμοποιηθεί σε προσαρμοσμένο κώδικα για να αποφασίσει πώς θα επεξεργαστεί ή πού θα αποθηκεύσει το αρχείο. |
| [KeepStreamOpen](../../aspose.tasks/resourcesavingargs/keepstreamopen/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ροή θα παραμείνει ανοιχτή μετά το τέλος της αποθήκευσης του πόρου. |
| [Stream](../../aspose.tasks/resourcesavingargs/stream/) { get; set; } | Λαμβάνει ή ορίζει το δυαδικό περιεχόμενο του αποθηκευμένου αρχείου. |
| [Uri](../../aspose.tasks/resourcesavingargs/uri/) { get; set; } | Λαμβάνει ή ορίζει το URI του πόρου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CloseStreamIfRequired](../../aspose.tasks/resourcesavingargs/closestreamifrequired/)() | Κλείστε τη ροή εάν το KeepStreamOpen είναι ψευδές, αλλιώς εκκαθαρίστε την. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τα επιχειρήματα αποθήκευσης γραμματοσειρών.

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

### Δείτε επίσης

* class [ResourceSavingArgs](../resourcesavingargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


