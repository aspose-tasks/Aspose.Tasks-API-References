---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "HtmlSaveOptions 생성자. HtmlSaveOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

[`HtmlSaveOptions`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public HtmlSaveOptions()
```

## 예제

프로젝트를 HTML 형식으로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// 또는

// 한 페이지만 추가 (페이지 번호 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### 또 보기

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


