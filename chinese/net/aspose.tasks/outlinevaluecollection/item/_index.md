---
title: "OutlineValueCollection.Item"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineValueCollection 属性。返回或设置指定索引处的元素"
type: docs
weight: 30
url: /zh/net/aspose.tasks/outlinevaluecollection/item/
---
## OutlineValueCollection indexer

返回或设置指定索引处的元素。

```csharp
public OutlineValue this[int index] { get; set; }
```

| 参数 | 描述 |
| --- | --- |
| index | 要获取或设置的元素的零基索引。 |

### 返回值

指定索引处的元素。

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

* class [OutlineValue](../../outlinevalue/)
* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


