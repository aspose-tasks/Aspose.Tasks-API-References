---
title: Class ProjectServerManager
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.ProjectServerManager 班级. 提供读取和执行指定 Project Online 帐户中项目或 指定本地 Project Server 实例支持 Project Server 2016 和 2019 版本中项目的方法的类
type: docs
weight: 1250
url: /zh/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

提供读取和执行指定 Project Online 帐户中项目或 指定本地 Project Server 实例（支持 Project Server 2016 和 2019 版本）中项目的方法的类。

```csharp
public sealed class ProjectServerManager
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | 初始化一个新的实例`ProjectServerManager`类. |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | 使用默认保存选项在 Project Server\Project Online 实例中创建新项目。 |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | 使用指定的保存选项在 Project Server\Project Online 实例中创建新项目。 |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | 从 Project Online 帐户\Project Server 实例获取具有指定 guid 的项目。 |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | 从当前 Project Online 帐户 \ Project Server 实例的“工作”存储中获取项目列表。 |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | 获取项目的二进制数据以进行故障排除。 |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | 使用默认保存选项更新 Project Server\Project Online 实例中的现有项目。现有项目将被覆盖。 |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | 使用指定的保存选项更新 Project Server\Project Online 实例中的现有项目。现有项目将被覆盖。 |

## 活动

| 姓名 | 描述 |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | 将 Web 请求发送到 Project Server 的 Web API 时引发的事件。 |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


