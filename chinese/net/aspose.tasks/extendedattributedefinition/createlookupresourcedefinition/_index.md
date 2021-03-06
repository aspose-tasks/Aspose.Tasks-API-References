---
title: CreateLookupResourceDefinition
second_title: Aspose.Tasks for .NET API 参考
description: 工厂方法它使用查找创建扩展属性定义 它有CalculationTypeaspose.tasks/extendedattributedefinition/calculationtype等于Lookup并且可以用于仅限资源 调用该方法时需要指定fieldId和alias 字段类型是从字段 id 推断出来的
type: docs
weight: 10
url: /zh/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

工厂方法，它使用查找创建扩展属性定义。 它有[`CalculationType`](../calculationtype)等于Lookup并且可以用于仅限资源。 调用该方法时需要指定*fieldId*和*alias*。 字段类型是从字段 id 推断出来的。

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | 指定的[`ExtendedAttributeResource`](../../extendedattributeresource)字段 ID。 |
| alias | String | 指定的String别名。 |

### 返回值

创建[`ExtendedAttributeDefinition`](../../extendedattributedefinition)类的实例，指定*fieldId*和*别名*。

### 例子

使用此示例为具有查找功能的资源创建自定义字段定义，然后用文本值填充它:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### 也可以看看

* enum [ExtendedAttributeResource](../../extendedattributeresource)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition)
* 部件 [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

工厂方法，它使用查找创建扩展属性定义。 它有[`CalculationType`](../calculationtype)等于Lookup并且可以用于仅限资源。 调用该方法时需要指定*customFieldType*,*fieldId*和*alias*。

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| customFieldType | CustomFieldType | 指定的[`CustomFieldType`](../../customfieldtype)类型。 |
| fieldId | ExtendedAttributeResource | 指定的[`ExtendedAttributeResource`](../../extendedattributeresource)字段 ID。 |
| alias | String | 指定的String别名。 |

### 返回值

创建[`ExtendedAttributeDefinition`](../../extendedattributedefinition)类的实例，指定*customFieldType*,*fieldId*和*alias*。

### 例子

使用此示例为具有查找功能的资源创建自定义字段定义，然后用文本值填充它:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### 也可以看看

* enum [CustomFieldType](../../customfieldtype)
* enum [ExtendedAttributeResource](../../extendedattributeresource)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition)
* 部件 [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
