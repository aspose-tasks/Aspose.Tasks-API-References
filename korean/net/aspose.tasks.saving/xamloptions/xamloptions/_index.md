---
title: "XamlOptions.XamlOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "XamlOptions 생성자. 프로젝트를 XAML 형식으로 저장하는 데 사용할 수 있는 XamlOptions 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

프로젝트를 XAML 형식으로 저장하는 데 사용할 수 있는 [`XamlOptions`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public XamlOptions()
```

## 예제

저장 옵션을 사용하여 프로젝트를 XAML 형식으로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### 또 보기

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


