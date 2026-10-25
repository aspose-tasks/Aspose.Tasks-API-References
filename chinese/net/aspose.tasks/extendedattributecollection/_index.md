---
title: "类 ExtendedAttributeCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ExtendedAttributeCollection 类。表示一个 ExtendedAttribute 对象的集合"
type: docs
weight: 530
url: /zh/net/aspose.tasks/extendedattributecollection/
---
## ExtendedAttributeCollection class

表示一个 [`ExtendedAttribute`](../extendedattribute/) 对象的集合。

```csharp
public class ExtendedAttributeCollection : IList<ExtendedAttribute>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributecollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/extendedattributecollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [Item](../../aspose.tasks/extendedattributecollection/item/) { get; set; } | 获取或设置指定索引处的元素。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributecollection/add/)(ExtendedAttribute) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/extendedattributecollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/extendedattributecollection/contains/)(ExtendedAttribute) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/extendedattributecollection/copyto/)(ExtendedAttribute[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/extendedattributecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [IndexOf](../../aspose.tasks/extendedattributecollection/indexof/)(ExtendedAttribute) | 确定此集合中指定项的索引。 |
| [Insert](../../aspose.tasks/extendedattributecollection/insert/)(int, ExtendedAttribute) | 在指定索引处插入指定项。 |
| [Remove](../../aspose.tasks/extendedattributecollection/remove/)(ExtendedAttribute) | 从此集合中移除特定对象的第一次出现。 |
| [RemoveAt](../../aspose.tasks/extendedattributecollection/removeat/)(int) | 在指定索引处移除一项。 |

## 示例

展示如何使用扩展属性集合。

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// 获取索引为零的任务
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // 清除扩展属性
    task.ExtendedAttributes.Clear();
}

// 为任务创建扩展属性定义
var taskDefinition1 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
var taskDefinition2 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Finish, ExtendedAttributeTask.Finish7, "Finish 7");
project.ExtendedAttributes.Add(taskDefinition1);
project.ExtendedAttributes.Add(taskDefinition2);

Console.WriteLine("Iterate over task extended attributes of " + task.Get(Tsk.Name) + " task: ");
foreach (var attribute in task.ExtendedAttributes)
{
    Console.WriteLine("Attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

// 添加扩展属性 1
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// 添加扩展属性 2
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// 使用扩展属性...

// 按索引移除扩展属性
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// 使用集合索引访问
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// 将属性复制到其他项目
var attributes = new ExtendedAttribute[task.ExtendedAttributes.Count];
task.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherTask.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other task's extended attributes: ");
foreach (var attribute in otherTask.ExtendedAttributes)
{
    Console.WriteLine("Other attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Other attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

if (task.ExtendedAttributes.Contains(extendedAttribute2))
{
    task.ExtendedAttributes.Remove(extendedAttribute2);
}

// 移除所有扩展属性定义
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### 另见

* class [ExtendedAttribute](../extendedattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


