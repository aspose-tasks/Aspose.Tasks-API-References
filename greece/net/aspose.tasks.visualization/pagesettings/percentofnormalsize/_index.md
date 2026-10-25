---
title: "PageSettings.PercentOfNormalSize"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageSettings. Λαμβάνει ή ορίζει ένα ποσοστό του κανονικού μεγέθους για προσαρμογή της εκτύπωσης"
type: docs
weight: 90
url: /el/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

Λαμβάνει ή ορίζει ένα ποσοστό του κανονικού μεγέθους για προσαρμογή της εκτύπωσης.

```csharp
public int PercentOfNormalSize { get; set; }
```

## Παραδείγματα

Εμφανίζει πώς να αποδοθεί η προβολή με τον καθορισμένο συντελεστή κλίμακας.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// ορίστε μια τιμή που υποδεικνύει ότι η προβολή πρέπει να κλιμακωθεί χρησιμοποιώντας τον καθορισμένο συντελεστή κλίμακας
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// καθορίστε τον συντελεστή κλίμακας
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### Δείτε επίσης

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


