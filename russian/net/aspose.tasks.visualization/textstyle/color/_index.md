---
title: "TextStyle.Color"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TextStyle. Получает или задает цвет текста"
type: docs
weight: 40
url: /ru/net/aspose.tasks.visualization/textstyle/color/
---
## TextStyle.Color property

Получает или задает цвет текста.

```csharp
public Color Color { get; set; }
```

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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


