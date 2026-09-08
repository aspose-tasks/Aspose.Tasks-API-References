---
title: "Класс PageViewSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.PageViewSettings. Представляет настройки печати для представления проекта"
type: docs
weight: 3260
url: /ru/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

Представляет настройки печати для представления проекта.

```csharp
public class PageViewSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | Получает или задает количество первых столбцов, которые будут печататься на всех страницах. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | Получает или задает значение, указывающее, следует ли подгонять временную шкалу к концу страницы при печати. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | Получает или задает значение, указывающее, следует ли печатать все столбцы листа представления. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | Получает или задает значение, указывающее, следует ли печатать пустые страницы представления. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | Получает или задает значение, указывающее, следует ли печатать указанное количество первых столбцов на всех страницах. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | Получает или задает значение, указывающее, следует ли печатать заметки. |

## Примеры

Показывает, как печатать заметки задач, ресурсов и назначений на отдельной странице.

```csharp
var project = new Project(DataDir + "Input.mpp");

// установить количество первых столбцов, печатаемых на всех страницах
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// установите значение, указывающее, следует ли печатать заметки.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// установите значение, указывающее, следует ли подгонять временную шкалу к концу страницы при печати.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// установите значение, указывающее, следует ли печатать все столбцы листа представления
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// установите значение, указывающее, следует ли печатать пустые страницы представления
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// установить значение, указывающее, печатать ли указанное количество первых столбцов на всех страницах
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


