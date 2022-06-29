---
title: CreateExtendedAttribute
second_title: Aspose.Tasks for .NET API 参考
description: 创建一个新的扩展属性其字段 ID 等于该对象的字段 ID 值
type: docs
weight: 300
url: /zh/net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## CreateExtendedAttribute() {#createextendedattribute}

创建一个新的扩展属性，其字段 ID 等于该对象的字段 ID 值。

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

### 返回值

返回创建的[`ExtendedAttribute`](../../extendedattribute)类实例，其 fieldID 等于此对象的 fieldID 值。

### 也可以看看

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition)
* 部件 [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(string) {#createextendedattribute_6}

创建一个新的扩展属性，其字段 ID 等于该对象的字段 ID 值和指定的文本值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| textValue | String | 指定的文本值。 |

### 返回值

返回创建的[`ExtendedAttribute`](../../extendedattribute)类实例，其 fieldID 等于该对象的 fieldID 值。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidOperationException | 如果当前[`CfType`](../cftype)不是 'Text' |

### 也可以看看

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition)
* 部件 [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(decimal) {#createextendedattribute_5}

创建一个新的扩展属性，其字段 ID 等于该对象的字段 ID 值和指定的数值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| numericValue | Decimal | 指定的数值。 |

### 返回值

返回创建的[`ExtendedAttribute`](../../extendedattribute)类实例，其 fieldID 等于该对象的 fieldID 值。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidOperationException | 如果当前[`CfType`](../cftype)不是“数字”或“成本” |

### 也可以看看

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition)
* 部件 [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(DateTime) {#createextendedattribute_4}

创建一个新的扩展属性，其字段 ID 等于该对象的字段 ID 值和指定的日期值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| dateTimeValue | DateTime | 指定的日期时间值。 |

### 返回值

返回创建的[`ExtendedAttribute`](../../extendedattribute)类实例，其 fieldID 等于该对象的 fieldID 值。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidOperationException | 如果当前[`CfType`](../cftype)不是“日期”，“开始”或“完成” |

### 也可以看看

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition)
* 部件 [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Duration) {#createextendedattribute_1}

创建一个新的扩展属性，其字段 ID 等于该对象的字段 ID 值和指定的持续时间值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| durationValue | Duration | 指定的持续时间值。 |

### 返回值

返回创建的[`ExtendedAttribute`](../../extendedattribute)类实例，其 fieldID 等于该对象的 fieldID 值。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidOperationException | 如果当前[`CfType`](../cftype)不是 'Duration' |

### 也可以看看

* class [ExtendedAttribute](../../extendedattribute)
* struct [Duration](../../duration)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition)
* 部件 [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(bool) {#createextendedattribute_3}

创建一个新的扩展属性，其字段 ID 等于该对象的字段 ID 值和指定的标志值。

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| flagValue | Boolean | 指定的标志值。 |

### 返回值

返回创建的[`ExtendedAttribute`](../../extendedattribute)类实例，其 fieldID 等于该对象的 fieldID 值。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidOperationException | 如果当前[`CfType`](../cftype)不是“标志” |

### 也可以看看

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition)
* 部件 [Aspose.Tasks](../../../)

---

## CreateExtendedAttribute(Value) {#createextendedattribute_2}

创建与指定[`Value`](../../value)项目链接的新扩展属性。

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| lookupValue | Value | 指定的[`Value`](../../value)项。 |

### 返回值

返回与指定链接的[`ExtendedAttribute`](../../extendedattribute)类的创建实例[`Value`](../../value)项目。

### 评论

*lookupValue*应该预先添加到[`ExtendedAttributeDefinition`](../../extendedattributedefinition)使用[`AddLookupValue`](../addlookupvalue)方法。

### 例子

使用此代码创建新[`ExtendedAttribute`](../../extendedattribute)使用特定值:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

### 也可以看看

* class [ExtendedAttribute](../../extendedattribute)
* class [Value](../../value)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* 命名空间 [Aspose.Tasks](../../extendedattributedefinition)
* 部件 [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
