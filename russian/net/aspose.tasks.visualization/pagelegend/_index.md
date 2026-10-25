---
title: "Класс PageLegend"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.PageLegend. Представляет легенду страницы, которая используется для печати проекта"
type: docs
weight: 3210
url: /ru/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

Представляет легенду страницы, используемую для печати проекта.

```csharp
public class PageLegend : HeaderFooterInfo
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageLegend](pagelegend/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Получает или задает центрированное изображение, отображаемое в родительском элементе. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Получает или задает отображаемый размер центрированного изображения. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Получает или задает центрированный текст для отображения в родительском элементе. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Получает или задает изображение, выровненное по левому краю, которое будет отображаться в родительском элементе. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Получает или задает отображаемый размер левого изображения. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Получает или задает текст, выровненный по левому краю, для отображения в родительском элементе. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | Получает или задает страницы, на которых отображается легенда. Может принимать одно из значений перечисления [`Legend`](../legend/). |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Получает или задает изображение, выровненное по правому краю, которое будет отображаться в родительском элементе. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Получает или задает отображаемый размер правого изображения. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Получает или задает текст, выровненный по правому краю, для отображения в родительском элементе. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | Получает или задает ширину левой части (по умолчанию содержащей название проекта и дату) легенды в сантиметрах. |

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

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


