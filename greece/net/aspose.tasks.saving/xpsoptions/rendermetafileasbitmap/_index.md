---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα XpsOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν ένα metafile πρέπει να αποδοθεί ως bitmap"
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν ένα μετααρχείο πρέπει να αποδοθεί ως bitmap.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως αρχείο XPS.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// δημιουργία επιλογών αποθήκευσης XPS και ρύθμιση των παραμέτρων
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### Δείτε επίσης

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


