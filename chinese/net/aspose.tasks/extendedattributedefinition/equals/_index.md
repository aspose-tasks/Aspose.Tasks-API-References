---
title: "ExtendedAttributeDefinition.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttributeDefinition 方法。返回一个标志，指示此实例是否等于指定的对象"
type: docs
weight: 320
url: /zh/net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

返回一个标志，指示此实例是否等于指定的对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 用于与此实例比较的指定对象。 |

### 返回值

一个标志，指示此实例是否等于指定的对象。

## 示例

展示如何检查扩展属性定义的相等性。

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// 日历的相等性是根据属性定义字段 ID 进行检查的。
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### 另见

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


