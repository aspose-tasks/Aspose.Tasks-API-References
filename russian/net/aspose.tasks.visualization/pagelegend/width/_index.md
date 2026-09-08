---
title: "PageLegend.Width"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageLegend. Получает или задает ширину левой части, содержащей название проекта и дату, по умолчанию легенды, в сантиметрах"
type: docs
weight: 30
url: /ru/net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

Получает или задает ширину левой части (по умолчанию содержащей название проекта и дату) легенды в сантиметрах.

```csharp
public double Width { get; set; }
```

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | При попытке установить значение меньше 0. |

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


