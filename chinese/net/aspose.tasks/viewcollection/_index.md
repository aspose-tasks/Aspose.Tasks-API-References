---
title: "类 ViewCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ViewCollection 类。包含 View 对象的列表。实现 ICollectionView 接口"
type: docs
weight: 2900
url: /zh/net/aspose.tasks/viewcollection/
---
## ViewCollection class

包含一个 [`View`](../view/) 对象列表。实现 ICollection&lt;View&gt; 接口。

```csharp
public class ViewCollection : ICollection<View>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | 获取 View 对象的父对象。只读 [`Project`](../project/)。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | 搜索具有指定名称的 View，并返回集合中的首次出现。 |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | 搜索具有指定 Screen 属性的 View，并返回集合中的首次出现。 |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | 从此集合中移除特定对象的第一次出现。 |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | 将视图集合转换为 [`View`](../view/) 对象列表。 |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


