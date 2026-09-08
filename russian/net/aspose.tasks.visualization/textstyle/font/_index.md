---
title: "TextStyle.Font"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TextStyle. Получает или задает шрифт стиля текста"
type: docs
weight: 50
url: /ru/net/aspose.tasks.visualization/textstyle/font/
---
## TextStyle.Font property

Получает или задает шрифт стиля текста.

```csharp
public FontDescriptor Font { get; set; }
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

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


