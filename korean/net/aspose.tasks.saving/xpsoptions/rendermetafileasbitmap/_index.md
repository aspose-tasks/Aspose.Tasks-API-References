---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Aspose.Tasks for .NET API 참조"
description: "XpsOptions 속성. 메타파일을 비트맵으로 렌더링할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

메타파일을 비트맵으로 렌더링할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
```

## 예제

프로젝트를 XPS 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// XPS 저장 옵션을 생성하고 매개변수를 조정합니다.
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### 또 보기

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


