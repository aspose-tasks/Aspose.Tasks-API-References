---
title: "SaveOptions.IsPortrait"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "SaveOptions‑Eigenschaft. Lässt einen Wert zu, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist."
type: docs
weight: 70
url: /de/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Liest oder setzt einen Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist.

```csharp
public bool IsPortrait { get; set; }
```

## Hinweise

Ist nicht anwendbar, wenn SaveOptions.PageSize == Visualization.PageSize.DefinedInView. In diesem Fall wird View.PageInfo.PageSettings.IsPortrait stattdessen verwendet. Ist nicht anwendbar, wenn SaveOptions.CustomPageSize gesetzt ist.

## Beispiele

Zeigt, wie die Seitengröße und -orientierung mithilfe von View‑Einstellungen oder SaveOptions festgelegt werden kann.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// In diesem Fall werden die Seitengröße und -orientierung aus den Eigenschaften view.PageInfo.PageSettings.PaperSize und view.PageInfo.PageSettings.IsPortrait übernommen.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// In diesem Fall werden die Seitengröße und -orientierung aus den Eigenschaften von SaveOptions übernommen.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// In diesem Fall wird die Seitengröße aus SaveOptions.CustomPageSize übernommen. Die IsPortrait‑Eigenschaft wird nicht berücksichtigt.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Siehe auch

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


