---
title: "类 WBSCodeMaskCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WBSCodeMaskCollection 类。表示 WBSCodeMask 对象的集合"
type: docs
weight: 3510
url: /zh/net/aspose.tasks/wbscodemaskcollection/
---
## WBSCodeMaskCollection class

表示一组 WBSCodeMask 对象。

```csharp
public class WBSCodeMaskCollection : IList<WBSCodeMask>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/wbscodemaskcollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/wbscodemaskcollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/wbscodemaskcollection/add/)(WBSCodeMask) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/wbscodemaskcollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/wbscodemaskcollection/contains/)(WBSCodeMask) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/wbscodemaskcollection/copyto/)(WBSCodeMask[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/wbscodemaskcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/wbscodemaskcollection/remove/)(WBSCodeMask) | 从此集合中移除特定对象的第一次出现。 |
| [ToList](../../aspose.tasks/wbscodemaskcollection/tolist/)() | 将 WBSCodeMaskCollection 转换为 [`WBSCodeMask`](../wbscodemask/) 对象的列表。 |

## 示例

展示如何使用 WBS 代码掩码集合。

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

project.WBSCodeDefinition.CodeMaskCollection.Clear();

var mask1 = new WBSCodeMask();
mask1.Length = 2;
mask1.Separator = "-";
mask1.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask1);

var mask2 = new WBSCodeMask();
mask2.Length = 1;
mask2.Separator = "-";
mask2.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask2);

Console.WriteLine("WBS Code mask's count: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
Console.WriteLine("Is WBS Code mask collection read-only?: " + project.WBSCodeDefinition.CodeMaskCollection.IsReadOnly);
Console.WriteLine("Masks: ");
Console.WriteLine();
foreach (var wbsMask in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var task1 = project.RootTask.Children.Add("Task 1");
task1.Children.Add("Task 2");

project.Recalculate();

IEnumerable<Task> childTasks = project.RootTask.SelectAllChildTasks();
foreach (var childTask in childTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}

project.WBSCodeDefinition.CodeMaskCollection.Remove(mask2);

if (project.WBSCodeDefinition.CodeMaskCollection.Contains(mask2))
{
    throw new InvalidOperationException("WBS code mask wasn't removed.");
}

var otherProject = new Project();
otherProject.WBSCodeDefinition = new WBSCodeDefinition();
otherProject.WBSCodeDefinition.GenerateWBSCode = true;
otherProject.WBSCodeDefinition.VerifyUniqueness = true;
otherProject.WBSCodeDefinition.CodePrefix = "CRS-";

// 复制代码掩码到其他项目
var masks = new WBSCodeMask[project.WBSCodeDefinition.CodeMaskCollection.Count];
project.WBSCodeDefinition.CodeMaskCollection.CopyTo(masks, 0);

foreach (var mask in masks)
{
    otherProject.WBSCodeDefinition.CodeMaskCollection.Add(mask);
}

List<WBSCodeMask> wbsMasks = otherProject.WBSCodeDefinition.CodeMaskCollection.ToList();
foreach (var wbsMask in wbsMasks)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var otherTask1 = project.RootTask.Children.Add("Other task 1");
otherTask1.Children.Add("Other task 2");

otherProject.Recalculate();

Console.WriteLine("Print WBS codes of the other project: ");
IEnumerable<Task> otherChildTasks = otherProject.RootTask.SelectAllChildTasks();
foreach (var childTask in otherChildTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}
```

### 另见

* class [WBSCodeMask](../wbscodemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


