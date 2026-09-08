---
title: "PageSettings.PercentOfNormalSize"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageSettings. Получает или задает процент от нормального размера для корректировки печати."
type: docs
weight: 90
url: /ru/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

Получает или задает процент от нормального размера, до которого следует корректировать печать.

```csharp
public int PercentOfNormalSize { get; set; }
```

## Примеры

Показывает, как отрисовать представление с указанным коэффициентом масштабирования.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// установить значение, указывающее, что представление должно масштабироваться с использованием указанного коэффициента масштабирования
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// указать коэффициент масштабирования
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### См. также

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


