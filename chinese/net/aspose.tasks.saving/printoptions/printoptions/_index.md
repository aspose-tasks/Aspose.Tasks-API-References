---
title: "PrintOptions.PrintOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrintOptions 构造函数。初始化 PrintOptions 类的新实例，可用于设置打印项目的不同选项"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

初始化 [`PrintOptions`](../) 类的新实例，可用于设置打印项目的不同选项。

```csharp
public PrintOptions()
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

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


