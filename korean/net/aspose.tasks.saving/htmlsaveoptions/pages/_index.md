---
title: "HtmlSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API 참조"
description: "HtmlSaveOptions 속성. 프로젝트 레이아웃을 렌더링할 때 저장할 페이지 번호 목록을 가져오거나 설정합니다. 이 목록이 비어 있으면 모든 프로젝트 페이지가 저장됩니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks.saving/htmlsaveoptions/pages/
---
## HtmlSaveOptions.Pages property

프로젝트 레이아웃을 렌더링할 때 저장할 페이지 번호 목록을 가져오거나 설정합니다. 이 목록이 비어 있으면 모든 프로젝트 페이지가 저장됩니다.

```csharp
public List<int> Pages { get; set; }
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


