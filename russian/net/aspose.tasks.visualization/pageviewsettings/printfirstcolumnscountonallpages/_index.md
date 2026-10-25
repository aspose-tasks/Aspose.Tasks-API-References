---
title: "PageViewSettings.PrintFirstColumnsCountOnAllPages"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageViewSettings. Получает или задает значение, указывающее, следует ли печатать указанное количество первых столбцов на всех страницах"
type: docs
weight: 60
url: /ru/net/aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/
---
## PageViewSettings.PrintFirstColumnsCountOnAllPages property

Получает или задает значение, указывающее, следует ли печатать указанное количество первых столбцов на всех страницах.

```csharp
public bool PrintFirstColumnsCountOnAllPages { get; set; }
```

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

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


