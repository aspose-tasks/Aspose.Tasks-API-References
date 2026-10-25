---
title: "PageSettings.PagesInHeight"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PageSettings. Ottiene o imposta il numero di pagine in altezza da stampare"
type: docs
weight: 50
url: /it/net/aspose.tasks.visualization/pagesettings/pagesinheight/
---
## PageSettings.PagesInHeight property

Ottiene o imposta il numero di pagine in altezza da stampare.

```csharp
public int PagesInHeight { get; set; }
```

## Esempi

Mostra come renderizzare la vista con l'opzione 'Adatta X a Y pagine'.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// specifica che la vista deve essere renderizzata in 2 pagine o meno in altezza
view.PageInfo.PageSettings.PagesInHeight = 2;
// specifica che la vista deve essere renderizzata in 1 pagina in larghezza
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

### Vedi anche

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


