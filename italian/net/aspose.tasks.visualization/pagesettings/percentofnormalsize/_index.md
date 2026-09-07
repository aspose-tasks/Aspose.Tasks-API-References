---
title: "PageSettings.PercentOfNormalSize"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PageSettings. Ottiene o imposta una percentuale della dimensione normale per regolare la stampa."
type: docs
weight: 90
url: /it/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

Ottiene o imposta una percentuale della dimensione normale a cui regolare la stampa.

```csharp
public int PercentOfNormalSize { get; set; }
```

## Esempi

Mostra come renderizzare la vista con il fattore di scala specificato.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// imposta un valore che indica che la vista deve essere scalata usando il fattore di scala specificato
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// specifica il fattore di scala
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### Vedi anche

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


