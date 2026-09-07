---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PageSettings. Ottiene o imposta un valore che indica se regolare la stampa alla percentuale specificata PercentOfNormalSize della dimensione normale"
type: docs
weight: 20
url: /it/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

Ottiene o imposta un valore che indica se regolare la stampa alla percentuale specificata ([`PercentOfNormalSize`](../percentofnormalsize/)) della dimensione normale.

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## Osservazioni

Non è efficace quando il progetto è renderizzato in formato HTML.

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


