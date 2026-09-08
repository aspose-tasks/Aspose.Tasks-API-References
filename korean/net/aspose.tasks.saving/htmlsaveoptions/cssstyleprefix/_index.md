---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Aspose.Tasks for .NET API 참조"
description: "HtmlSaveOptions 속성. CSS 스타일 접두사를 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

CSS 스타일 접두사를 가져오거나 설정합니다.

```csharp
public string CssStylePrefix { get; set; }
```

## 예제

HTML로 내보낼 때 사용되는 CSS 스타일에 대한 공통 접두사를 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### 또 보기

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


