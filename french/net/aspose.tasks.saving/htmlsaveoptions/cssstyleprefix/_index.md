---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit le préfixe de style CSS"
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

Obtient ou définit le préfixe de style CSS.

```csharp
public string CssStylePrefix { get; set; }
```

## Exemples

Montre comment définir un préfixe commun pour les styles CSS utilisés lors de l'exportation vers HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


