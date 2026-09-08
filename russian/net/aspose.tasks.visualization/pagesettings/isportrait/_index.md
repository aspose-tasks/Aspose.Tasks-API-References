---
title: "PageSettings.IsPortrait"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageSettings. Получает или задает значение, указывающее, является ли ориентация страницы портретной; возвращает false, если ориентация страницы альбомная."
type: docs
weight: 40
url: /ru/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

Получает или задает значение, указывающее, является ли ориентация страницы портретной; возвращает false, если ориентация страницы альбомная.

```csharp
public bool IsPortrait { get; set; }
```

## Примечания

Применяется при рендеринге, когда SaveOptions.PageSize == Visualization.PageSize.DefinedInView.

## Примеры

Показывает, как работать с &lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// получить настройки
var settings = project.DefaultView.PageInfo.PageSettings;
// давайте настроим некоторые свойства
// установите значение, указывающее, является ли ориентация страницы портретной; возвращает false, если ориентация страницы альбомная.
settings.IsPortrait = true;
// установите количество страниц по ширине для печати.
settings.PagesInWidth = 5;
// установите количество страниц по высоте для печати.
settings.PagesInHeight = 7;
// установите процент от нормального размера, до которого следует корректировать печать.
settings.PercentOfNormalSize = 200;
// установите размер бумаги. Может быть одним из значений перечисления <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" />.
settings.PaperSize = PrinterPaperSize.PaperB4;
// установите номер первой страницы для печати.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

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

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


