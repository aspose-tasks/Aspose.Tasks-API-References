---
title: "ViewCollection.Contains"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ViewCollection 方法。若在此集合中找到指定项则返回 true，否则返回 false"
type: docs
weight: 60
url: /zh/net/aspose.tasks/viewcollection/contains/
---
## ViewCollection.Contains method

如果在此集合中找到指定项则返回 true；否则返回 false。

```csharp
public bool Contains(View item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | View | 要查找的指定项。 |

### 返回值

如果在此集合中找到指定项则返回 true；否则返回 false。

## 示例

展示如何使用视图集合。

```csharp
var project = new Project(DataDir + "Project1.mpp");

// 转换为普通视图列表
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// 添加新视图
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// 遍历视图
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// 一次性删除所有视图
project.Views.Clear();

// 或逐个删除
{
    // 方法 1
    List<View> listToDelete = project.Views.ToList();
    foreach (var v in listToDelete)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}

{
    // 方法 2
    var array = new View[project.Views.Count];
    project.Views.CopyTo(array, 0);
    foreach (var v in array)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}
```

### 另见

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


