---
title: "ProjectInfo.IsCheckedOut"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectInfo 属性。获取一个值，指示项目是否已签出。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/projectinfo/ischeckedout/
---
## ProjectInfo.IsCheckedOut property

获取一个值，指示项目是否已签出。

```csharp
public bool IsCheckedOut { get; }
```

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

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


