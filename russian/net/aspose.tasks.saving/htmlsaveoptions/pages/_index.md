---
title: "HtmlSaveOptions.Pages"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство HtmlSaveOptions. Получает или задает список номеров страниц для сохранения при рендеринге макета проекта. Все страницы проекта будут сохранены, если этот список пуст."
type: docs
weight: 130
url: /ru/net/aspose.tasks.saving/htmlsaveoptions/pages/
---
## HtmlSaveOptions.Pages property

Получает или задает список номеров страниц для сохранения при рендеринге макета проекта. Если список пуст, будут сохранены все страницы проекта.

```csharp
public List<int> Pages { get; set; }
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


