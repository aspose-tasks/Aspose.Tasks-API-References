---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfSaveOptions 생성자. PDF 형식으로 문서를 저장하는 데 사용할 수 있는 PdfSaveOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

[`PdfSaveOptions`](../) 클래스의 새 인스턴스를 초기화합니다. 이 클래스를 사용하면 문서를 [`PDF`](../../savefileformat/) 형식으로 저장할 수 있습니다.

```csharp
public PdfSaveOptions()
```

## 예제

프로젝트의 선택된 페이지를 PDF 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// 내보낼 수 있는 페이지 수를 확인해 봅시다
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### 또 보기

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


