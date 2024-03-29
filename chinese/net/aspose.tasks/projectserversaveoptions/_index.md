---
title: Class ProjectServerSaveOptions
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.ProjectServerSaveOptions 班级. 允许在将项目保存到 Project Server 或 Project Online 时指定其他选项
type: docs
weight: 1260
url: /zh/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

允许在将项目保存到 Project Server 或 Project Online 时指定其他选项。

```csharp
public sealed class ProjectServerSaveOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | 初始化一个新的实例`ProjectServerSaveOptions`类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | 获取或设置队列作业状态请求之间的间隔。默认值为 2 秒。 |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | 获取或设置项目的唯一标识符。在 Project Server\Project Online 实例中应该是唯一的。 |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | 获取或设置显示在 Project Server\Project Online 项目列表中的项目名称。在 Project Server\Project Online 实例中应该是唯一的。 如果省略该值，将使用 Prj.Name 属性的值代替。 |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | 获取或设置在等待 Project Server 的队列处理服务处理保存项目请求时使用的超时。此属性的默认值为 1 分钟。 |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


