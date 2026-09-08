---
title: "TextStyle.ItemType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TextStyle. Получает или задает TextItemType стиля текста"
type: docs
weight: 60
url: /ru/net/aspose.tasks.visualization/textstyle/itemtype/
---
## TextStyle.ItemType property

Получает или задает [`TextItemType`](../../textitemtype/) стиля текста.

```csharp
public virtual TextItemType ItemType { get; set; }
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

* enum [TextItemType](../../textitemtype/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


