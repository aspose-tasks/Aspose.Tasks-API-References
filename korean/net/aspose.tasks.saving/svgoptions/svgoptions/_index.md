---
title: "SvgOptions.SvgOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SvgOptions 생성자. 프로젝트를 SVG 형식으로 저장하는 데 사용할 수 있는 SvgOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/svgoptions/svgoptions/
---
## SvgOptions constructor

`[`SvgOptions`](../)` 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 프로젝트를 SVG 형식으로 저장하는 데 사용할 수 있습니다.

```csharp
public SvgOptions()
```

## 예제

프로젝트를 SVG 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // 문서가 저장될 <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />을 설정합니다.
                            PresentationFormat = PresentationFormat.GanttChart,

                            // 행 높이를 내용에 맞게 늘릴지 여부를 나타내는 값을 설정합니다.
                            FitContent = true,

                            // 렌더링할 최소 시간 기간을 설정합니다. 기본값은 <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Days</see>입니다.
                            Timescale = Timescale.ThirdsOfMonths,

                            // 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 결정합니다.
                            // 현재 SVG로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### 또 보기

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


