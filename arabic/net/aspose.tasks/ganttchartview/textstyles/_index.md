---
title: "GanttChartView.TextStyles"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GanttChartView. تحصل أو تعيّن قائمة من TextStyle لعرض مخطط جانت"
type: docs
weight: 170
url: /ar/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

تحصل أو تعيّن قائمة من [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) لعرض مخطط جانت.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## الأمثلة

يظهر كيفية قراءة أنماط نص مخطط جانت.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// التكرار عبر أنماط النص في عرض مخطط جانت
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### انظر أيضًا

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


