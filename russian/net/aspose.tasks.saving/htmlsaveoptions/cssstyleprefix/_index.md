---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство HtmlSaveOptions. Получает или задает префикс CSS-стилей"
type: docs
weight: 30
url: /ru/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

Получает или задает префикс CSS‑стилей.

```csharp
public string CssStylePrefix { get; set; }
```

## Примеры

Показывает, как задать общий префикс для CSS-стилей, используемых при экспорте в HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


