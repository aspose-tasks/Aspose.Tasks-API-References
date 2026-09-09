---
title: "ProjectServerManager"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 870
url: /zh/python-net/aspose.tasks/projectservermanager/
---

## ProjectServerManager class

此类提供读取和对指定 Project Online 帐户中的项目或<br/>            指定本地 Project Server 实例中的项目执行操作的方法（支持 Project Server 2016 和 2019 版本）。

ProjectServerManager 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| ProjectServerManager(credentials) | 初始化 [ProjectServerManager](/tasks/python-net/aspose.tasks/projectservermanager/) 类的新实例。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| update_project(project) | 使用默认保存选项更新 Project Server\Project Online 实例中的现有项目。现有项目将被覆盖。 |
| update_project(project, save_options) | 使用指定的保存选项更新 Project Server\Project Online 实例中的现有项目。现有项目将被覆盖。 |
| create_new_project(project) | 使用默认保存选项在 Project Server\Project Online 实例中创建新项目。 |
| create_new_project(project, save_options) | 使用指定的保存选项在 Project Server\Project Online 实例中创建新项目。 |
| get_project(project_guid) | 从 Project Online 帐户\Project Server 实例中获取具有指定 guid 的项目。 |
| get_project_raw_data(project_guid) | 获取项目的二进制数据以用于故障排除。 |
| get_project_list() | 从当前 Project Online 帐户\Project Server 实例的“Working”存储中获取项目列表。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

