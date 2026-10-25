---
title: "类 ResourceCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ResourceCollection 类。表示 Resource 对象的集合"
type: docs
weight: 1770
url: /zh/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

表示一个 [`Resource`](../resource/) 对象的集合。

```csharp
public class ResourceCollection : IList<Resource>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | 获取 ResourceCollection 中包含的元素数量。只读 Int32。 |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | 返回指定索引处的元素。 |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | 获取 ResourceCollection 对象的父项目。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | 在项目资源集合的最后位置添加新资源。 |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | 在项目资源集合的最后位置添加新资源。 |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | 在项目资源集合的指定位置添加新资源。 |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | 不支持直接清除，此方法仅抛出 NotSupportedException。 |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | 返回具有指定 id 的资源。 |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | 返回具有指定 Uid 的资源。 |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | 这是 ICollection 的 Remove 方法的存根实现，仅抛出 NotSupportedException。 |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | 将 ResourceCollection 对象转换为 [`Resource`](../resource/) 对象的列表。 |

## 示例

展示如何使用资源集合。

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// 添加空资源
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// 添加带名称的资源
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// 在具有指定 ID 的资源之前添加资源
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// 按 id 获取资源
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// 资源集合不支持 Clear 操作
// project.Resources.Clear();
// 使用下一个代码示例代替
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### 另见

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


