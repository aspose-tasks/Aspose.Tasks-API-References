---
title: "UsageView.DisplayDetailsHeaderColumn"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство UsageView. Получает или задает значение, указывающее, отображать ли столбец заголовка деталей в представлении или нет"
type: docs
weight: 30
url: /ru/net/aspose.tasks/usageview/displaydetailsheadercolumn/
---
## UsageView.DisplayDetailsHeaderColumn property

Получает или задает значение, указывающее, отображать ли столбец заголовка деталей в представлении или нет.

```csharp
public bool DisplayDetailsHeaderColumn { get; set; }
```

## Примеры

Показывает, как отобразить представление использования задач с деталями.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// получить представление
UsageView view = (TaskUsageView)project.DefaultView;

// столбец заголовка деталей не будет отображаться
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// отобразить столбец заголовка деталей
view.DisplayDetailsHeaderColumn = true;

// повторять заголовок деталей во всех строках назначений
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### См. также

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


