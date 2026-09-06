---
title: "Rsc.WindowsUserAccount"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。与资源关联的 NT 帐户"
type: docs
weight: 680
url: /zh/net/aspose.tasks/rsc/windowsuseraccount/
---
## Rsc.WindowsUserAccount field

与资源关联的 NT 帐户。

```csharp
public static readonly Key<string, RscKey> WindowsUserAccount;
```

## 示例

展示如何设置资源的元属性。

```csharp
var project = new Project(DataDir + "Project.mpp");

// 添加资源并设置资源元数据
var resource = project.Resources.Add("Rsc 1");
resource.Set(Rsc.EMailAddress, "1@gmail.com");
resource.Set(Rsc.WindowsUserAccount, "user_acc1");
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


