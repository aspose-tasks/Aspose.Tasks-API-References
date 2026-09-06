---
title: "类 ProjectInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ProjectInfo 类。关于在 Project Online 上可用的已发布项目的简要信息"
type: docs
weight: 1470
url: /zh/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

关于在 Project Online 上可用的已发布项目的简要信息。

```csharp
public sealed class ProjectInfo
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ProjectInfo](projectinfo/)() | 初始化 `ProjectInfo` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | 获取项目创建的日期和时间。 |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | 获取项目的描述。 |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | 获取项目的唯一标识符。 |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | 获取一个值，指示项目是否已签出。 |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | 获取项目最近一次发布的日期。 |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | 获取项目最近一次保存的日期。 |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | 获取项目的名称。 |

## 示例

展示如何从 Project Online 读取项目信息。

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// 读取项目信息
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


