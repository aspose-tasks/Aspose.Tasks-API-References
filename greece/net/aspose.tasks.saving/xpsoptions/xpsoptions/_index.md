---
title: "XpsOptions.XpsOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής XpsOptions. Αρχικοποιεί μια νέα παρουσία της κλάσης XpsOptions"
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XpsOptions`](../).

```csharp
public XpsOptions()
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


