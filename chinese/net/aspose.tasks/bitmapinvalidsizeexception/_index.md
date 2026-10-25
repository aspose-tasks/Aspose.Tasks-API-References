---
title: "类 BitmapInvalidSizeException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.BitmapInvalidSizeException 类。表示在内存不足以创建位图实例时发生的异常"
type: docs
weight: 140
url: /zh/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

表示在内存不足以创建位图实例时发生的异常。

```csharp
public class BitmapInvalidSizeException : Exception
```

## 示例

展示如何将项目保存为图像并捕获无效大小异常。

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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


