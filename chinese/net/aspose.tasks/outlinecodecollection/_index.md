---
title: "类 OutlineCodeCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OutlineCodeCollection 类。表示 OutlineCode 对象的集合。"
type: docs
weight: 1160
url: /zh/net/aspose.tasks/outlinecodecollection/
---
## OutlineCodeCollection class

表示一个 [`OutlineCode`](../outlinecode/) 对象的集合。

```csharp
public class OutlineCodeCollection : IList<OutlineCode>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodecollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/outlinecodecollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [Item](../../aspose.tasks/outlinecodecollection/item/) { get; set; } | 返回或设置指定索引处的元素。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodecollection/add/)(OutlineCode) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/outlinecodecollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/outlinecodecollection/contains/)(OutlineCode) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/outlinecodecollection/copyto/)(OutlineCode[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/outlinecodecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [IndexOf](../../aspose.tasks/outlinecodecollection/indexof/)(OutlineCode) | 确定此集合中指定项的索引。 |
| [Insert](../../aspose.tasks/outlinecodecollection/insert/)(int, OutlineCode) | 在指定索引处插入指定项。 |
| [Remove](../../aspose.tasks/outlinecodecollection/remove/)(OutlineCode) | 从此集合中移除特定对象的第一次出现。 |
| [RemoveAt](../../aspose.tasks/outlinecodecollection/removeat/)(int) | 在指定索引处移除一项。 |

## 示例

展示如何使用大纲代码集合。

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

for (var i = 0; i < collector.Tasks.Count; i++)
{
    var current = collector.Tasks[i];
    if (current.Get(Tsk.Id) == 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes for the " + current.Get(Tsk.Name) + " task.");
    Console.WriteLine("Count of outline codes: " + current.OutlineCodes.Count);
    foreach (var outlineCode in current.OutlineCodes)
    {
        Console.WriteLine("Field Id: " + outlineCode.FieldId);
        Console.WriteLine("Value Id: " + outlineCode.ValueId);
        Console.WriteLine("Value Guid: " + outlineCode.ValueGuid);
        Console.WriteLine();
    }
}

// 添加自定义大纲代码定义。
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
project.OutlineCodes.Add(outlineCodeDefinition);

// 创建大纲代码。
var value = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(value);

var codeOne = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 1, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

var task = project.RootTask.Children.GetByUid(2);

// 可以检查集合不是只读的。
if (!task.OutlineCodes.IsReadOnly)
{
    task.OutlineCodes.Add(codeOne);
}

var codeZero = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 0, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

task.OutlineCodes.Insert(0, codeZero);

var code2 = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 2, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

// 在错误的位置插入代码 2。
task.OutlineCodes.Insert(0, code2);

// 修复它。
var indexOf = task.OutlineCodes.IndexOf(code2);
task.OutlineCodes.RemoveAt(indexOf);

// 在正确的位置插入代码 2。
task.OutlineCodes.Insert(2, code2);

// 检查代码已被插入。
Console.WriteLine("Is outline codes contains the inserted value: " + task.OutlineCodes.Contains(code2));

// ...
// 使用大纲代码。
// ...
var otherProject = new Project(DataDir + "OutlineCodes2003.mpp");
var otherTask = otherProject.RootTask.Children.GetById(2);

// 添加自定义大纲代码定义。
outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
otherProject.OutlineCodes.Add(outlineCodeDefinition);

// 创建大纲代码。
var otherValue = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(otherValue);

var outlineCodes = new OutlineCode[task.OutlineCodes.Count];
task.OutlineCodes.CopyTo(outlineCodes, 0);

foreach (var code in outlineCodes)
{
    otherTask.OutlineCodes.Add(code);
}

// ...
// 使用大纲代码。
// ...

// 移除大纲代码。
otherTask.OutlineCodes.RemoveAt(0);

while (otherTask.OutlineCodes.Count > 0)
{
    otherTask.OutlineCodes.Remove(otherTask.OutlineCodes[0]);
}

// 一次性清除所有值。
task.OutlineCodes.Clear();
```

### 另见

* class [OutlineCode](../outlinecode/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


