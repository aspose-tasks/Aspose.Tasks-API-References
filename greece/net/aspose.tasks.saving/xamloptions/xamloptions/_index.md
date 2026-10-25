---
title: "XamlOptions.XamlOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής XamlOptions. Αρχικοποιεί μια νέα παρουσία της κλάσης XamlOptions που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή XAML"
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XamlOptions`](../) που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή XAML.

```csharp
public XamlOptions()
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο σε μορφή XAML χρησιμοποιώντας επιλογές αποθήκευσης.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### Δείτε επίσης

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


