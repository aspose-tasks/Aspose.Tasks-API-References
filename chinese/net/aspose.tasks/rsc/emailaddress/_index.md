---
title: "Rsc.EMailAddress"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源的电子邮件地址"
type: docs
weight: 280
url: /zh/net/aspose.tasks/rsc/emailaddress/
---
## Rsc.EMailAddress field

资源的电子邮件地址。

```csharp
public static readonly Key<string, RscKey> EMailAddress;
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


