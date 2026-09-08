---
title: "클래스 BitmapInvalidSizeException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.BitmapInvalidSizeException class. 비트맵 인스턴스를 생성할 메모리가 충분하지 않을 때 발생하는 예외를 나타냅니다."
type: docs
weight: 140
url: /ko/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

비트맵 인스턴스를 생성할 메모리가 충분하지 않을 때 발생하는 예외를 나타냅니다.

```csharp
public class BitmapInvalidSizeException : Exception
```

## 예제

프로젝트를 이미지로 저장하고 잘못된 크기 예외를 포착하는 방법을 보여줍니다.

```csharp
try
{
    var project = new Project(DataDir + "Blank2010.mpp");

    GanttChartView view = (GanttChartView) project.Views.ToList()[0];
    var options = new ImageSaveOptions(SaveFileFormat.Png)
    {
        Timescale = Timescale.DefinedInView
    };

    view.MiddleTimescaleTier.Unit = TimescaleUnit.Minutes;
    view.MiddleTimescaleTier.Count = 1;

    project.Save(OutDir + "SaveToStreamAndCatchException_out.mpp", options);
}
catch (BitmapInvalidSizeException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


