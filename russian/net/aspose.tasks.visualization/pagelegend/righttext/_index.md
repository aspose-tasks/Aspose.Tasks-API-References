---
title: "PageLegend.RightText"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageLegend. Получает или задает выровненный по правому краю текст, отображаемый в легенде страницы"
type: docs
weight: 80
url: /ru/net/aspose.tasks.visualization/pagelegend/righttext/
---
## PageLegend.RightText property

Получает или задает выровненный по правому краю текст, отображаемый в легенде страницы.

```csharp
public string RightText { get; set; }
```

## Примеры

Показывает, как работать с информацией о легенде страницы.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// давайте прочитаем информацию о легенде страницы
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// также поддерживается изменение легенды
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


