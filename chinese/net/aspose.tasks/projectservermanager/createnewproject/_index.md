---
title: ProjectServerManager.CreateNewProject
second_title: Aspose.Tasks for .NET API 参考
description: ProjectServerManager 方法. 使用默认保存选项在 Project ServerProject Online 实例中创建新项目
type: docs
weight: 30
url: /zh/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

使用默认保存选项在 Project Server\Project Online 实例中创建新项目。

```csharp
public void CreateNewProject(Project project)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 要保存到 Project Server\Project Online 实例的项目。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 在通信错误或服务器返回错误的情况下。 |

### 例子

在此示例中，项目从 .mpp 文件加载并保存到 Project Online 帐户。

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "密码");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

### 也可以看看

* class [Project](../../project/)
* class [ProjectServerManager](../)
* 命名空间 [Aspose.Tasks](../../projectservermanager/)
* 部件 [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

使用指定的保存选项在 Project Server\Project Online 实例中创建新项目。

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 要保存到 Project Server\Project Online 实例的项目。 |
| saveOptions | ProjectServerSaveOptions | 的实例[`ProjectServerSaveOptions`](../../projectserversaveoptions/)班级。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 在通信错误或服务器返回错误的情况下。 |

### 例子

在此示例中，项目从 .mpp 文件加载并保存到 Project Online 帐户。

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "密码");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

### 也可以看看

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* 命名空间 [Aspose.Tasks](../../projectservermanager/)
* 部件 [Aspose.Tasks](../../../)


