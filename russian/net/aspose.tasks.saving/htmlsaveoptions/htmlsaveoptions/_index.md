---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор HtmlSaveOptions. Инициализирует новый экземпляр класса HtmlSaveOptions"
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

Инициализирует новый экземпляр класса [`HtmlSaveOptions`](../).

```csharp
public HtmlSaveOptions()
```

## Примеры

Показывает, как сохранить проект в формате HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// ИЛИ

// Добавление только одной страницы (страница номер 2).
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


