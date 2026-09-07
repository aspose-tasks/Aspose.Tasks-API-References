---
title: "FontSettings.FontResolveCallback"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα FontSettings. Λαμβάνει ή ορίζει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή των επιλυμένων γραμματοσειρών."
type: docs
weight: 30
url: /el/net/aspose.tasks/fontsettings/fontresolvecallback/
---
## FontSettings.FontResolveCallback property

Λαμβάνει ή ορίζει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή των επιλυμένων γραμματοσειρών.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένη κλήση επιστροφής επίλυσης γραμματοσειρών για να εκτελέσετε κώδικα που ορίζεται από τον χρήστη ώστε να ορίσετε εναλλακτική γραμματοσειρά ή να αντικαταστήσετε τη συγκεκριμένη γραμματοσειρά.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

options.FontSettings.FontResolveCallback = delegate(FontResolveEventArgs args)
{
    if (args.RequestedFontName != args.ResolvedFontName)
    {
        // Φαίνεται ότι η ακριβής γραμματοσειρά δεν μπορεί να βρεθεί και ορίστηκε εναλλακτική γραμματοσειρά.
        // Μπορούμε να παρακάμψουμε την εναλλακτική γραμματοσειρά.
        args.ResolvedFontName = "Arial";
    }

    // Ή απλώς αντικαταστήστε τη συγκεκριμένη γραμματοσειρά:
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### Δείτε επίσης

* delegate [FontResolveCallbackDelegate](../../fontresolvecallbackdelegate/)
* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


