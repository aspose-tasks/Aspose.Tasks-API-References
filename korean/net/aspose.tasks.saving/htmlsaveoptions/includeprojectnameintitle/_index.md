---
title: "HtmlSaveOptions.IncludeProjectNameInTitle"
second_title: "Aspose.Tasks for .NET API 참조"
description: "HtmlSaveOptions 속성. HTML 제목에 프로젝트 이름을 포함할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 120
url: /ko/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

HTML 제목에 프로젝트 이름을 포함할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool IncludeProjectNameInTitle { get; set; }
```

## 예제

&lt;see cref="P:Aspose.Tasks.Saving.HtmlSaveOptions" /&gt; 옵션을 사용하여 페이지 HTML 헤더/제목을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // 프로젝트 이름을 HTML 제목에 포함할지 여부를 결정합니다(기본값은 true).
    IncludeProjectNameInTitle = false,

    // 프로젝트 이름을 HTML 페이지 헤더에 포함할지 여부를 결정합니다(기본값은 true).
    IncludeProjectNameInPageHeader = false,

    // 내보낼 페이지를 설정합니다.
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### 또 보기

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


