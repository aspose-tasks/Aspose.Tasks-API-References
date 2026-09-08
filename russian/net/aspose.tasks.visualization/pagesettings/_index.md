---
title: "Класс PageSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.PageSettings. Представляет настройки печати для страницы представления проекта"
type: docs
weight: 3240
url: /ru/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

Представляет настройки печати для страницы представления проекта.

```csharp
public class PageSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageSettings](pagesettings/)() | Инициализирует новый экземпляр класса `PageSettings`. Представляет настройки печати для страницы представления проекта. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | Получает или задает значение, указывающее, следует ли корректировать печать до указанного процента ([`PercentOfNormalSize`](./percentofnormalsize/)) от нормального размера. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | Получает или задает номер первой страницы для печати. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | Получает или задает значение, указывающее, является ли ориентация страницы портретной; возвращает false, если ориентация страницы альбомная. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | Получает или задает количество страниц по высоте для печати. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | Получает или задает количество страниц по ширине для печати. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | Получает или задает размер бумаги. Может быть одним из значений перечисления [`PrinterPaperSize`](../printerpapersize/). |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | Получает или задает целое число, представляющее одно из значений PrinterPaperSize или идентификатор пользовательского размера страницы. Это значение можно использовать для получения PaperSize из настроек ОС. |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | Получает или задает процент от нормального размера, до которого следует корректировать печать. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


