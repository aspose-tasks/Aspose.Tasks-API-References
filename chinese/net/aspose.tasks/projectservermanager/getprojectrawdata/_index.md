---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerManager 方法。获取项目的二进制数据以用于故障排除。"
type: docs
weight: 60
url: /zh/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

获取项目的二进制数据以用于故障排除。

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectGuid | Guid | 要读取的项目的 Guid。 |

### 返回值

包含原始项目数据的流。

## 示例

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// 您尝试获取的项目的 GUID。
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

展示如何从 Microsoft Project Online 检索项目的原始数据以用于故障排除。

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);

    // 用户可以将项目作为原始数据流读取以用于故障排除。
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // 您可以将生成的文件提交给支持部门。
}
```

### 另见

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


