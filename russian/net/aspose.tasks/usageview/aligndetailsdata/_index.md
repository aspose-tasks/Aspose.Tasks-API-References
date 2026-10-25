---
title: "UsageView.AlignDetailsData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "UsageView свойство. Возвращает или задает выравнивание данных деталей"
type: docs
weight: 10
url: /ru/net/aspose.tasks/usageview/aligndetailsdata/
---
## UsageView.AlignDetailsData property

Получает или задает выравнивание данных деталей.

```csharp
public HorizontalStringAlignment AlignDetailsData { get; set; }
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

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


