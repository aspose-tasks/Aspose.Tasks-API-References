---
title: "SaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν πρέπει να χρησιμοποιηθεί gradient brush κατά την απόδοση του Gantt Chart."
type: docs
weight: 220
url: /el/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση του Gantt Chart.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## Παρατηρήσεις

Ισχύει μόνο όταν η προβολή Gantt chart αποδίδεται.

## Παραδείγματα

Δείχνει πώς να ορίσετε μια τιμή που υποδεικνύει εάν πρέπει να χρησιμοποιηθεί gradient brush κατά την απόδοση του Gantt Chart.

```csharp
var project = new Project(DataDir + "Project2.mpp");

SaveOptions options = new XamlOptions
{
    UseGradientBrush = false
};
project.Save(OutDir + "ChangeGanttBarsColorGradient_Solid_out.xaml", options);

options.UseGradientBrush = true;
project.Save(OutDir + "ChangeGanttBarsColorGradient_Gradient_out.xaml", options);
```

### Δείτε επίσης

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


