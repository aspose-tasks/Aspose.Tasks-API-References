---
title: "SaveOptions.TextStyles"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 가져오거나 설정합니다."
type: docs
weight: 190
url: /ko/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

프로젝트 뷰 렌더링 중에 적용되는 텍스트 스타일 목록을 가져오거나 설정합니다.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## 비고

이러한 스타일은 GanttCharView.TextStyles에 정의된 스타일을 재정의합니다.

## 예제

프로젝트의 다양한 텍스트 항목을 스타일링하는 데 사용되는 저장 옵션의 텍스트 스타일 사용 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Bold | FontStyles.Italic)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};

project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### 또 보기

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


