---
title: "ResourceCollection.Clear"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceCollection 方法。直接清除不受支持，此方法仅抛出 NotSupportedException。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/resourcecollection/clear/
---
## ResourceCollection.Clear method

不支持直接清除，此方法仅抛出 NotSupportedException。

```csharp
public void Clear()
```

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

* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


