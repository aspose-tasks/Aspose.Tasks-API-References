---
title: "Перечисление BackgroundPattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.BackgroundPattern. Указывает шаблон фона"
type: docs
weight: 100
url: /ru/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

Указывает шаблон фона.

```csharp
public enum BackgroundPattern
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | Указывает темный диагональный левый шаблон фона. |
| DarkDiagonalRight | `8` | Указывает темный диагональный правый шаблон фона. |
| DarkDither | `13` | Указывает темный шумовой шаблон фона. |
| DarkFill | `4` | Указывает темный заливочный шаблон фона. |
| DiagonalLeft | `5` | Указывает диагональный левый шаблон фона. |
| DiagonalRight | `6` | Указывает диагональный правый шаблон фона. |
| Hollow | `0` | Указывает пустой шаблон фона. |
| LightDither | `11` | Указывает светлый шумовой шаблон фона. |
| LightFill | `2` | Указывает светлый заливочный шаблон фона. |
| MediumDither | `12` | Указывает средний шумовой шаблон фона. |
| MediumFill | `3` | Указывает средний заливочный шаблон фона. |
| MediumVerticalStripe | `10` | Указывает средний вертикальный полосатый шаблон фона. |
| SolidFill | `1` | Указывает сплошной заливочный шаблон фона. |
| ThinVerticalStripe | `9` | Указывает тонкий вертикальный полосатый шаблон фона. |

## Примеры

Показывает, как настраивать стили текста, которые используются для оформления различных текстовых элементов в проекте.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


