---
title: "PageSettings.PageSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PageSettings. Инициализирует новый экземпляр класса PageSettings. Представляет параметры печати для страницы представления проекта."
type: docs
weight: 10
url: /ru/net/aspose.tasks.visualization/pagesettings/pagesettings/
---
## PageSettings constructor

Инициализирует новый экземпляр класса [`PageSettings`](../). Представляет параметры печати для страницы представления проекта.

```csharp
public PageSettings()
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

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


