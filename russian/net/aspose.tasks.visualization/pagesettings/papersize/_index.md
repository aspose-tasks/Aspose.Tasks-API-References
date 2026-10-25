---
title: "PageSettings.PaperSize"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageSettings. Получает или задает размер бумаги. Может принимать одно из значений перечисления PrinterPaperSize."
type: docs
weight: 70
url: /ru/net/aspose.tasks.visualization/pagesettings/papersize/
---
## PageSettings.PaperSize property

Получает или задает размер бумаги. Может принимать одно из значений перечисления [`PrinterPaperSize`](../../printerpapersize/).

```csharp
public PrinterPaperSize PaperSize { get; set; }
```

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

### См. также

* enum [PrinterPaperSize](../../printerpapersize/)
* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


