---
title: "GanttChartView.TextStyles"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство GanttChartView. Получает или задаёт список TextStyle представления диаграммы Ганта"
type: docs
weight: 170
url: /ru/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Получает или задаёт список [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) представления диаграммы Ганта.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Примеры

Показывает, как читать стили текста диаграммы Ганта.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// перебор стилей текста представления диаграммы Ганта
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### См. также

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


