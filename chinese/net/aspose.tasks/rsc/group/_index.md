---
title: "Rsc.Group"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源所属的组"
type: docs
weight: 300
url: /zh/net/aspose.tasks/rsc/group/
---
## Rsc.Group field

资源所属的组。

```csharp
public static readonly Key<string, RscKey> Group;
```

## 示例

展示如何处理资源费率和组。

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// 添加资源并设置一些属性
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


