---
title: "PageSettings.PagesInHeight"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PageSettings. Λαμβάνει ή ορίζει έναν αριθμό σελίδων σε ύψος που θα εκτυπωθούν"
type: docs
weight: 50
url: /el/net/aspose.tasks.visualization/pagesettings/pagesinheight/
---
## PageSettings.PagesInHeight property

Λαμβάνει ή ορίζει τον αριθμό των σελίδων σε ύψος που θα εκτυπωθούν.

```csharp
public int PagesInHeight { get; set; }
```

## Παραδείγματα

Εμφανίζει πώς να αποδοθεί η προβολή με την επιλογή 'Προσαρμογή X σε Y σελίδες'.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// καθορίστε ότι η προβολή πρέπει να αποδοθεί σε 2 σελίδες ή λιγότερο σε ύψος
view.PageInfo.PageSettings.PagesInHeight = 2;
// καθορίστε ότι η προβολή πρέπει να αποδοθεί σε 1 σελίδα σε πλάτος
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### Δείτε επίσης

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


