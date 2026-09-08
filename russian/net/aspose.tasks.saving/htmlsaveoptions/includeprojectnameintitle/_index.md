---
title: "HtmlSaveOptions.IncludeProjectNameInTitle"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство HtmlSaveOptions. Получает или задает значение, указывающее, включать ли имя проекта в заголовок HTML."
type: docs
weight: 120
url: /ru/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

Получает или задает значение, указывающее, включать ли название проекта в заголовок HTML.

```csharp
public bool IncludeProjectNameInTitle { get; set; }
```

## Примеры

Показывает, как задать заголовок/титул HTML-страницы, используя параметры &lt;see cref="P:Aspose.Tasks.Saving.HtmlSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // Определяет, включать ли имя проекта в заголовок HTML (по умолчанию true)
    IncludeProjectNameInTitle = false,

    // Определяет, включать ли имя проекта в заголовок HTML-страницы (по умолчанию true)
    IncludeProjectNameInPageHeader = false,

    // установить страницы, которые будут экспортированы
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


