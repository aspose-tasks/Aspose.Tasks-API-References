---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源的 Active Directory Guid"
type: docs
weight: 20
url: /zh/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

资源的 Active Directory Guid。

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## 示例

展示如何读取/写入 Rsc.ActiveDirectoryGuid 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


