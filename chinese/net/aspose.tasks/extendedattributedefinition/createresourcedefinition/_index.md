---
title: ExtendedAttributeDefinition.CreateResourceDefinition
second_title: Aspose.Tasks for .NET API 参考
description: ExtendedAttributeDefinition 方法. 创建简单扩展属性定义的工厂方法Microsoft Project 显示为无 它具有CalculationType等于None并且只能在资源中使用 您需要指定customFieldTypefieldId和alias调用此方法时.
type: docs
weight: 30
url: /zh/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

创建简单扩展属性定义的工厂方法，Microsoft Project 显示为“无”。 它具有[`CalculationType`](../calculationtype/)等于None并且只能在资源中使用。 您需要指定*customFieldType*,*fieldId*和*alias*调用此方法时.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| customFieldType | CustomFieldType | 指定的[`CustomFieldType`](../../customfieldtype/)类型。 |
| fieldId | ExtendedAttributeResource | 指定的[`ExtendedAttributeResource`](../../extendedattributeresource/)字段标识。 |
| alias | String | 指定的String别名。 |

### 返回值

创建的实例[`ExtendedAttributeDefinition`](../)指定类*customFieldType*,*fieldId*和*alias*.

### 例子

使用此示例创建自定义文本字段定义：

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### 也可以看看

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition/)
* 部件 [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

创建简单扩展属性定义的工厂方法，Microsoft Project 显示为“无”。 它具有[`CalculationType`](../calculationtype/)等于None并且只能在资源中使用。 您需要指定*fieldId*和*alias*当调用这个方法时。 字段类型是从字段id推断出来的。

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | 指定的[`ExtendedAttributeResource`](../../extendedattributeresource/)字段标识。 |
| alias | String | 指定的String别名。 |

### 返回值

创建的实例[`ExtendedAttributeDefinition`](../)指定类*fieldId*和*alias*.

### 例子

使用此示例创建自定义文本字段定义：

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### 也可以看看

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition/)
* 部件 [Aspose.Tasks](../../../)


