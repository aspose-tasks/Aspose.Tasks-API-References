---
title: "类 LoadOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.LoadOptions 类。允许在从文件或流加载项目时指定额外的加载参数"
type: docs
weight: 990
url: /zh/net/aspose.tasks/loadoptions/
---
## LoadOptions class

允许在从文件或流加载项目时指定附加加载参数。

```csharp
public class LoadOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [LoadOptions](loadoptions/)() | 初始化 `LoadOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | 获取或设置可用于取消项目加载操作的令牌。 |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | 获取或设置用于从 HTML、MPX、XER 和 Primavera XML 格式读取项目的编码。默认编码为 UTF8。 |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | 获取或设置处理 XML 解析错误的回调方法。 |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | 获取或设置保护密码。 |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | 获取或设置 [`PrimaveraReadOptions`](../primaverareadoptions/) 类的指定实例，可用于自定义加载 Primavera 格式（Primavera P6 XER 或 Primavera P6 Xml）的行为。 |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | 获取或设置在项目加载操作期间调用的回调。目前支持 MPP 和 XER 格式。 |

## 示例

展示如何使用 &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; 实例加载受密码保护的项目。

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


