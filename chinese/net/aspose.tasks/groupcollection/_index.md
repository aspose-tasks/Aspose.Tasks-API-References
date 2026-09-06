---
title: "类 GroupCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.GroupCollection 类。包含 Group 对象的列表。实现 ICollectionGroup 接口"
type: docs
weight: 780
url: /zh/net/aspose.tasks/groupcollection/
---
## GroupCollection class

包含一个 [`Group`](../group/) 对象列表。实现 ICollection&lt;Group&gt; 接口。

```csharp
public class GroupCollection : ICollection<Group>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | 从此集合中移除特定对象的第一次出现。 |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | 将组集合转换为 [`Group`](../group/) 对象列表。 |

## 示例

展示如何使用组集合。

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// 遍历任务组
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// 遍历资源组
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// 清除其他项目的组
otherProject.TaskGroups.Clear();

// 将组复制到其他项目
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// 添加自定义任务组
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// 移除所有组
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### 另见

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


