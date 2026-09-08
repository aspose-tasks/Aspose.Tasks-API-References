---
title: "ImageSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ImageSaveOptions 속성. 프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 가져오거나 설정합니다. 이 목록이 비어 있으면 모든 페이지가 저장됩니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 가져오거나 설정합니다. 이 목록이 비어 있으면 모든 페이지가 저장됩니다.

```csharp
public List<int> Pages { get; set; }
```

## 예제

선택한 페이지를 이미지로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### 또 보기

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


