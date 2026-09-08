---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageSettings. Получает или задает значение, указывающее, следует ли корректировать печать до указанного процента PercentOfNormalSize от нормального размера."
type: docs
weight: 20
url: /ru/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

Получает или задает значение, указывающее, следует ли корректировать печать до указанного процента ([`PercentOfNormalSize`](../percentofnormalsize/)) от нормального размера.

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## Примечания

Не действует, когда проект отрисован в формате HTML.

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


