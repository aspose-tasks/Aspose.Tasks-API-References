---
title: "Класс HeaderFooterInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.HeaderFooterInfo. Представляет визуальное содержимое верхнего/нижнего колонтитула или легенды, используемое для печати и визуализации представлений"
type: docs
weight: 3130
url: /ru/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

Представляет визуальное содержимое заголовка, нижнего колонтитула или легенды, используемое для печати \ отображения представлений.

```csharp
public class HeaderFooterInfo
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | Инициализирует новый экземпляр класса `HeaderFooterInfo`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Получает или задает центрированное изображение, отображаемое в родительском элементе. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Получает или задает отображаемый размер центрированного изображения. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Получает или задает центрированный текст для отображения в родительском элементе. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Получает или задает изображение, выровненное по левому краю, которое будет отображаться в родительском элементе. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Получает или задает отображаемый размер левого изображения. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Получает или задает текст, выровненный по левому краю, для отображения в родительском элементе. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Получает или задает изображение, выровненное по правому краю, которое будет отображаться в родительском элементе. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Получает или задает отображаемый размер правого изображения. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Получает или задает текст, выровненный по правому краю, для отображения в родительском элементе. |

## Примеры

Показывает, как считывать информацию заголовка/нижнего колонтитула страницы.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


