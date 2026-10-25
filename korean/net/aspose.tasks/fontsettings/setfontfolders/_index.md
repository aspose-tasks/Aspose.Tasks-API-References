---
title: "FontSettings.SetFontFolders"
second_title: "Aspose.Tasks for .NET API 참조"
description: "FontSettings 메서드. 프로젝트 뷰를 렌더링할 때 Aspose.Tasks가 TrueType 글꼴을 찾는 폴더를 설정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

프로젝트 뷰를 렌더링할 때 Aspose.Tasks가 TrueType 글꼴을 찾는 폴더를 설정합니다.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fontFolders | String[] | TrueType 글꼴을 포함하는 폴더들의 배열입니다. |
| recursive | Boolean | true인 경우 지정된 폴더를 재귀적으로 스캔합니다. |

## 예제

사용자 지정 글꼴 폴더를 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// 열린 프로젝트에서 사용되는 모든 글꼴의 TrueType 파일은 MyFonts 폴더에 있어야 합니다.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### 또 보기

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


