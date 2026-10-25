---
title: "GroupCollection.Contains"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GroupCollection 方法。若在此集合中找到指定项则返回 true，否则返回 false"
type: docs
weight: 50
url: /zh/net/aspose.tasks/groupcollection/contains/
---
## GroupCollection.Contains method

如果在此集合中找到指定项则返回 true；否则返回 false。

```csharp
public bool Contains(Group item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | Group | 要查找的指定项。 |

### 返回值

如果在此集合中找到指定项则返回 true；否则返回 false。

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

* class [Group](../../group/)
* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


