---
title: "PageSettings.PagesInHeight"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageSettings. Получает или задает количество страниц по высоте для печати."
type: docs
weight: 50
url: /ru/net/aspose.tasks.visualization/pagesettings/pagesinheight/
---
## PageSettings.PagesInHeight property

Получает или задает количество страниц по высоте для печати.

```csharp
public int PagesInHeight { get; set; }
```

## Примеры

Показывает, как отрисовать представление с опцией «Fit X to Y pages».

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// указать, что представление должно быть отрисовано в 2 страницах или менее по высоте
view.PageInfo.PageSettings.PagesInHeight = 2;
// указать, что представление должно быть отрисовано в 1 странице по ширине
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### См. также

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


