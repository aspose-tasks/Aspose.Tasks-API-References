---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti HtmlSaveOptions. Mendapatkan atau mengatur awalan gaya CSS"
type: docs
weight: 30
url: /id/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

Mendapatkan atau mengatur awalan gaya CSS.

```csharp
public string CssStylePrefix { get; set; }
```

## Contoh

Menampilkan cara mengatur awalan umum untuk gaya CSS yang digunakan selama ekspor ke HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### Lihat Juga

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


