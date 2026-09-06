---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttributeDefinition 方法。返回 ExtendedAttributeDefinition 类实例的哈希码"
type: docs
weight: 330
url: /zh/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

返回 [`ExtendedAttributeDefinition`](../) 类实例的哈希码。

```csharp
public override int GetHashCode()
```

### 返回值

此对象的哈希码。

## 示例

展示如何获取扩展属性定义的哈希码。

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// 扩展属性定义的哈希码等于字段 ID。
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### 另见

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


