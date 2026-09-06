---
title: "类 ApsLayoutBuilderOutOfMemoryException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException 类。表示在内存不足以继续图像布局构建时发生的异常"
type: docs
weight: 20
url: /zh/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

表示在内存不足以继续图像布局构建时出现的异常。

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## 示例

展示如何将项目保存为图像并捕获异常。

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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


