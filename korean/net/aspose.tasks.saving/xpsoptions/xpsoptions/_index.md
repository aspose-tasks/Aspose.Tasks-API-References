---
title: "XpsOptions.XpsOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "XpsOptions 생성자. XpsOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

`[`XpsOptions`](../)` 클래스의 새 인스턴스를 초기화합니다.

```csharp
public XpsOptions()
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


