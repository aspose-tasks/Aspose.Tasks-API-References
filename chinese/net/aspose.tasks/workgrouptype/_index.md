---
title: "枚举 WorkGroupType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WorkGroupType 枚举。指定工作组的类型"
type: docs
weight: 3620
url: /zh/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

指定工作组的类型。

```csharp
public enum WorkGroupType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Default | `0` | 指示默认工作组类型。 |
| None | `1` | 指示无工作组类型。 |
| Email | `2` | 指示电子邮件工作组类型。 |
| Web | `3` | 指示网络工作组类型。 |

## 示例

展示如何设置资源的工作组。

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


