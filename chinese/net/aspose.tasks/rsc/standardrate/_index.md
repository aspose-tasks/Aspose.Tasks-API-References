---
title: "Rsc.StandardRate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源执行的常规非加班工作的工资率"
type: docs
weight: 620
url: /zh/net/aspose.tasks/rsc/standardrate/
---
## Rsc.StandardRate field

资源执行的常规非加班工作薪酬率。

```csharp
public static readonly Key<decimal, RscKey> StandardRate;
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


