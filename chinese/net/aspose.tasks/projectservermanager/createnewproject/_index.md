---
title: "ProjectServerManager.CreateNewProject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerManager 方法。使用默认保存选项在 Project ServerProject Online 实例中创建新项目。"
type: docs
weight: 30
url: /zh/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

使用默认保存选项在 Project Server\\Project Online 实例中创建新项目。

```csharp
public void CreateNewProject(Project project)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 要保存到 Project Server\\Project Online 实例的项目。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 如果出现通信错误或服务器返回的错误。 |

## 示例

在此示例中，项目从 .mpp 文件加载并保存到 Project Online 账户。

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

展示如何使用 ProjectServerManager 在 Microsoft Project Online 上创建新项目。

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 另见

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

使用指定的保存选项在 Project Server\Project Online 实例中创建新项目。

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 要保存到 Project Server\\Project Online 实例的项目。 |
| saveOptions | ProjectServerSaveOptions | [`ProjectServerSaveOptions`](../../projectserversaveoptions/) 类的实例。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 如果出现通信错误或服务器返回的错误。 |

## 示例

在此示例中，项目从 .mpp 文件加载并保存到 Project Online 账户。

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

展示如何使用 Project Server 管理器在 Microsoft Project Online 上使用预定义的保存选项创建新项目。

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 另见

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


