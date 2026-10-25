---
title: "SaveOptions.TextStyles"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает список стилей текста, применяемых при рендеринге представления проекта"
type: docs
weight: 190
url: /ru/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

Получает или задает список стилей текста, применяемых при отрисовке представления проекта.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Примечания

Эти стили переопределяют стили, определённые в GanttCharView.TextStyles.

## Примеры

Показывает, как использовать стили текста параметров сохранения, которые применяются для стилизации различных **text** элементов в проекте.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Bold | FontStyles.Italic)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};

project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### См. также

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


