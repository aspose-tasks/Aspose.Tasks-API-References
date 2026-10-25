---
title: "ViewCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ViewCollection 方法。返回此集合的枚举器"
type: docs
weight: 100
url: /zh/net/aspose.tasks/viewcollection/getenumerator/
---
## ViewCollection.GetEnumerator method

返回此集合的枚举器。

```csharp
public IEnumerator<View> GetEnumerator()
```

### 返回值

此集合的枚举器。

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


