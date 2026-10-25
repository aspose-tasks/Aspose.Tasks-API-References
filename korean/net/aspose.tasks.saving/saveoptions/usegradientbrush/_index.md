---
title: "SaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 그라디언트 브러시를 Gantt Chart 렌더링 시 사용할지 여부를 나타내는 값을 가져오거나 설정합니다"
type: docs
weight: 220
url: /ko/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Gantt 차트를 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## 비고

Gantt 차트 뷰가 렌더링될 때만 적용됩니다.

## 예제

그라디언트 브러시를 Gantt Chart 렌더링 시 사용할지 여부를 나타내는 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

SaveOptions options = new XamlOptions
{
    UseGradientBrush = false
};
project.Save(OutDir + "ChangeGanttBarsColorGradient_Solid_out.xaml", options);

options.UseGradientBrush = true;
project.Save(OutDir + "ChangeGanttBarsColorGradient_Gradient_out.xaml", options);
```

### 또 보기

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


