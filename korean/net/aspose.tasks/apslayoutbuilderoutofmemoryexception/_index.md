---
title: "클래스 ApsLayoutBuilderOutOfMemoryException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException 클래스. 이미지 레이아웃 구축을 계속할 메모리가 부족할 때 발생하는 예외를 나타냅니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

이미지 레이아웃 빌드를 계속할 메모리가 부족할 때 발생하는 예외를 나타냅니다.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## 예제

프로젝트를 이미지로 저장하고 예외를 처리하는 방법을 보여줍니다.

```csharp
try
{
    var project = new Project(DataDir + "Blank2010.mpp");

    var ganttChart = (GanttChartView)project.Views.ToList()[0];

    ganttChart.MiddleTimescaleTier.Unit = TimescaleUnit.Hours;
    ganttChart.BottomTimescaleTier.Unit = TimescaleUnit.Minutes;
    ganttChart.BottomTimescaleTier.Count = 1;

    var options = new ImageSaveOptions(SaveFileFormat.Png);
    options.Timescale = Timescale.DefinedInView;

    project.Save(OutDir + "SaveToStreamWithOptionsAndCatchException_out.mpp", options);
}
catch (ApsLayoutBuilderOutOfMemoryException ex)
{
    Console.WriteLine(ex.Message);
}
catch (BitmapInvalidSizeException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


