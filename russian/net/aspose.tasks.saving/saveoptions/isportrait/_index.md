---
title: "SaveOptions.IsPortrait"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает значение, указывающее, является ли ориентация страницы портретной; возвращает false, если ориентация страницы альбомная."
type: docs
weight: 70
url: /ru/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Получает или задает значение, указывающее, является ли ориентация страницы портретной; возвращает false, если ориентация страницы альбомная.

```csharp
public bool IsPortrait { get; set; }
```

## Примечания

Не применяется, когда SaveOptions.PageSize == Visualization.PageSize.DefinedInView. В этом случае используется View.PageInfo.PageSettings.IsPortrait. Не применяется, когда задано SaveOptions.CustomPageSize.

## Примеры

Показано, как указать размер и ориентацию страницы, используя настройки View или SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// В этом случае размер и ориентация страницы берутся из свойств view.PageInfo.PageSettings.PaperSize и view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// В этом случае размер и ориентация страницы берутся из свойств SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// В этом случае размер страницы берется из SaveOptions.CustomPageSize. Свойство IsPortrait не учитывается.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


