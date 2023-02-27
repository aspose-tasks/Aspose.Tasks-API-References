---
title: ExtendedAttributeDefinition.AddLookupValue
second_title: Aspose.Tasks for .NET API 参考
description: ExtendedAttributeDefinition 方法. 向内部查找列表添加一个值这是使用ValueList.
type: docs
weight: 290
url: /zh/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

向内部查找列表添加一个值。这是使用[`ValueList`](../valuelist/).

```csharp
public void AddLookupValue(Value value)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| value | Value | 要添加到查找中的值。 |

### 评论

此方法仅适用于[`ExtendedAttributeDefinition`](../)instances 其中有[`CalculationType`](../calculationtype/)等于Lookup.

### 例子

使用此代码将新值添加到查找列表：

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### 也可以看看

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition/)
* 部件 [Aspose.Tasks](../../../)


