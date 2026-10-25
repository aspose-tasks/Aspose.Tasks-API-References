---
title: "类 OutlineValueCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OutlineValueCollection 类。表示 OutlineValue 对象的集合。"
type: docs
weight: 1220
url: /zh/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

表示一个 [`OutlineValue`](../outlinevalue/) 对象的集合。

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读。 |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | 返回或设置指定索引处的元素。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | 确定此集合中指定项的索引。 |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | 在指定索引处插入指定项。 |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | 从此集合中移除特定对象的第一次出现。 |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | 在指定索引处移除一项。 |

## 示例

展示如何使用大纲值集合。

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// 清除值集合
foreach (var outlineCode in project.OutlineCodes)
{
    // 清除大纲掩码
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// 通过索引访问更新值
codeDefinition.Values[0].Value = "654321";

// 遍历大纲值
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// 使用大纲值
// ...

// 在需要时移除值
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// 在起始位置插入值
codeDefinition.Values.Insert(0, value);

// 检查已插入值的位置
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// 使用大纲值
// ...

// 从集合中移除最后一个值
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// 可以创建另一个大纲代码定义
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// 然后复制大纲值
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### 另见

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


