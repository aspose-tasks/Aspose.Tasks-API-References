---
title: "Resource.Set"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 方法。将指定属性映射到此容器中的指定值"
type: docs
weight: 860
url: /zh/net/aspose.tasks/resource/set/
---
## Set&lt;T&gt;(Key&lt;T, RscKey&gt;, T) {#set_1}

将指定属性映射到此容器中的指定值。

```csharp
public void Set<T>(Key<T, RscKey> key, T val)
```

| 参数 | 描述 |
| --- | --- |
| T | 映射值的类型。 |
| key | 指定的属性键。[`Rsc`](../../rsc/) 用于获取属性键。 |
| val | 该值。 |

## 示例

展示如何读取/写入常用资源属性。

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
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, RscKey&gt;, DateTime) {#set}

将指定属性映射到此容器中的指定值。

```csharp
public void Set(Key<DateTime, RscKey> key, DateTime val)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | Key`2 | 指定的属性键。[`Rsc`](../../rsc/) 用于获取属性键。 |
| val | DateTime | 该值。 |

## 示例

展示如何读取/写入常用资源属性。

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
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


