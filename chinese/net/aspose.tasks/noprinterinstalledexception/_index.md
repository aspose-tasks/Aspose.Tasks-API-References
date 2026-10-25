---
title: "类 NoPrinterInstalledException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.NoPrinterInstalledException 类。表示在操作系统中没有已安装打印机时抛出的异常"
type: docs
weight: 1100
url: /zh/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

表示在操作系统中未安装打印机时抛出的异常。

```csharp
public class NoPrinterInstalledException : Exception
```

## 示例

展示如何使用打印选项。

```csharp
try
{
    var project = new Project(DataDir + "Project2.mpp");
    var options = new PrintOptions
    {
        Timescale = Timescale.ThirdsOfMonths
    };
    if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
    {
        project.Print(options);
    }
}
catch (NoPrinterInstalledException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


