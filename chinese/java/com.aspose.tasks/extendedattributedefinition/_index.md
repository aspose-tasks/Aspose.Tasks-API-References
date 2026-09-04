---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示与项目关联的扩展属性定义。"
type: docs
weight: 83
url: /zh/java/com.aspose.tasks/extendedattributedefinition/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttributeDefinition
```

表示与项目关联的扩展属性定义。
## 方法

| 方法 | 描述 |
| --- | --- |
| [addLookupValue(Value value)](#addLookupValue-com.aspose.tasks.Value-) | 向内部查找列表添加一个值。 |
| [compareTo(ExtendedAttributeDefinition o)](#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-) | 比较此对象与另一个 @\\{code ExtendedAttributeDefinition\\} 类的实例。 |
| [createExtendedAttribute()](#createExtendedAttribute--) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值。 |
| [createExtendedAttribute(boolean flagValue)](#createExtendedAttribute-boolean-) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的标志值。 |
| [createExtendedAttribute(Duration durationValue)](#createExtendedAttribute-com.aspose.tasks.Duration-) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的持续时间值。 |
| [createExtendedAttribute(Value lookupValue)](#createExtendedAttribute-com.aspose.tasks.Value-) | 创建与指定的 [Value](../../com.aspose.tasks/value) 项关联的新扩展属性。 |
| [createExtendedAttribute(String textValue)](#createExtendedAttribute-java.lang.String-) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的文本值。 |
| [createExtendedAttribute(BigDecimal numericValue)](#createExtendedAttribute-java.math.BigDecimal-) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的数值。 |
| [createExtendedAttribute(Date dateTimeValue)](#createExtendedAttribute-java.util.Date-) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的日期值。 |
| [createLookupResourceDefinition(int customFieldType, int fieldId, String alias)](#createLookupResourceDefinition-int-int-java.lang.String-) | 创建带查找的扩展属性定义的工厂方法。 |
| [createLookupResourceDefinition(int fieldId, String alias)](#createLookupResourceDefinition-int-java.lang.String-) | 创建带查找的扩展属性定义的工厂方法。 |
| [createLookupTaskDefinition(int customFieldType, int fieldId, String alias)](#createLookupTaskDefinition-int-int-java.lang.String-) | 创建带查找的扩展属性定义的工厂方法。 |
| [createLookupTaskDefinition(int fieldId, String alias)](#createLookupTaskDefinition-int-java.lang.String-) | 创建带查找的扩展属性定义的工厂方法。 |
| [createResourceDefinition(int customFieldType, int fieldId, String alias)](#createResourceDefinition-int-int-java.lang.String-) | 创建简单扩展属性定义的工厂方法，Microsoft Project 将其显示为 "None"。 |
| [createResourceDefinition(int fieldId, String alias)](#createResourceDefinition-int-java.lang.String-) | 创建简单扩展属性定义的工厂方法，Microsoft Project 将其显示为 "None"。 |
| [createTaskDefinition(int customFieldType, int fieldId, String alias)](#createTaskDefinition-int-int-java.lang.String-) | 创建简单扩展属性定义的工厂方法，Microsoft Project 将其显示为 "None"。 |
| [createTaskDefinition(int fieldId, String alias)](#createTaskDefinition-int-java.lang.String-) | 创建简单扩展属性定义的工厂方法，Microsoft Project 将其显示为 "None"。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个标志，指示此实例是否等于指定的对象。 |
| [getAlias()](#getAlias--) | 获取自定义字段的别名。 |
| [getAppendNewValues()](#getAppendNewValues--) | 获取一个值，指示添加到项目的新值是否会自动添加到列表中。 |
| [getAutoRollDown()](#getAutoRollDown--) | 获取一个值，指示是否已启用对任务分配的自动向下滚动。 |
| [getCalculationType()](#getCalculationType--) | 获取自定义属性值的计算类型。 |
| [getCfType()](#getCfType--) | 获取自定义字段的类型。 |
| [getDefault()](#getDefault--) | 获取列表中的默认值。 |
| [getDefaultGuid()](#getDefaultGuid--) | 获取默认查找表条目的 Guid。 |
| [getElementType()](#getElementType--) | 获取扩展属性是否与任务、资源或分配关联。 |
| [getFieldId()](#getFieldId--) | 获取对应于自定义字段的项目 ID。 |
| [getFieldName()](#getFieldName--) | 获取自定义字段的名称。 |
| [getFormula()](#getFormula--) | 获取 Microsoft Project 用于填充自定义任务字段的公式。 |
| [getGraphicalIndicator()](#getGraphicalIndicator--) | 获取与扩展属性关联的图形指示器信息。 |
| [getGuid()](#getGuid--) | 获取自定义字段的 Guid。 |
| [getLookupUid()](#getLookupUid--) | 获取与自定义字段关联的查找表的 Guid。 |
| [getMaxMultiValues()](#getMaxMultiValues--) | 获取在下拉列表中可以设置的最大值数量。 |
| [getParentProject()](#getParentProject--) | 获取 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 实例的父项目。 |
| [getPhoneticsAlias()](#getPhoneticsAlias--) | 获取自定义字段别名的音标发音。 |
| [getRestrictValues()](#getRestrictValues--) | 获取一个值，指示自定义字段的值是否受限于 `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--))。 |
| [getRollupType()](#getRollupType--) | 获取汇总的计算方式。 |
| [getSecondaryGuid()](#getSecondaryGuid--) | 获取扩展属性的次要 guid。 |
| [getSecondaryPid()](#getSecondaryPid--) | 获取自定义字段的次要 PID。 |
| [getSummaryRowsCalculationType()](#getSummaryRowsCalculationType--) | 获取汇总行中自定义属性值的计算类型。 |
| [getUserDef()](#getUserDef--) | 获取一个值，指示自定义字段是否为用户定义。 |
| [getValueList()](#getValueList--) | 获取 List&lt;Value&gt; ValueList。 |
| [getValuelistSortOrder()](#getValuelistSortOrder--) | 获取值列表的排序方式。 |
| [hashCode()](#hashCode--) | 返回 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 类实例的哈希码。 |
| [removeLookupValue(Value value)](#removeLookupValue-com.aspose.tasks.Value-) | 从内部查找列表中移除一个值。 |
| [setAlias(String value)](#setAlias-java.lang.String-) | 设置自定义字段的别名。 |
| [setAppendNewValues(boolean value)](#setAppendNewValues-boolean-) | 设置一个值，指示是否将添加到项目的新值自动加入列表。 |
| [setAutoRollDown(boolean value)](#setAutoRollDown-boolean-) | 设置一个值，指示是否启用自动向任务分配下放。 |
| [setCalculationType(int value)](#setCalculationType-int-) | 设置自定义属性值的计算类型。 |
| [setDefault(String value)](#setDefault-java.lang.String-) | 设置列表中的默认值。 |
| [setDefaultGuid(String value)](#setDefaultGuid-java.lang.String-) | 设置默认查找表条目的 Guid。 |
| [setElementType(int value)](#setElementType-int-) | 设置扩展属性关联到任务、资源或分配。 |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | 设置对应于自定义字段的项目 ID。 |
| [setFormula(String value)](#setFormula-java.lang.String-) | 设置 Microsoft Project 用于填充自定义任务字段的公式。 |
| [setGraphicalIndicator(GraphicalIndicatorsInfo value)](#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-) | 设置与扩展属性关联的图形指示器信息。 |
| [setGuid(String value)](#setGuid-java.lang.String-) | 设置自定义字段的 Guid。 |
| [setMaxMultiValues(int value)](#setMaxMultiValues-int-) | 设置在下拉列表中可以设置的最大值数量。 |
| [setPhoneticsAlias(String value)](#setPhoneticsAlias-java.lang.String-) | 设置自定义字段别名的拼音发音。 |
| [setRestrictValues(boolean value)](#setRestrictValues-boolean-) | 设置一个值，指示自定义字段的值是否受限于 `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--))。 |
| [setRollupType(int value)](#setRollupType-int-) | 设置汇总的计算方式。 |
| [setSecondaryGuid(String value)](#setSecondaryGuid-java.lang.String-) | 设置扩展属性的次要 guid。 |
| [setSecondaryPid(String value)](#setSecondaryPid-java.lang.String-) | 设置自定义字段的次要 PID。 |
| [setSummaryRowsCalculationType(int value)](#setSummaryRowsCalculationType-int-) | 设置汇总行中自定义属性值的计算类型。 |
| [setUserDef(boolean value)](#setUserDef-boolean-) | 设置一个值，指示自定义字段是否为用户定义。 |
| [setValuelistSortOrder(int value)](#setValuelistSortOrder-int-) | 设置值列表的排序方式。 |
### addLookupValue(Value value) {#addLookupValue-com.aspose.tasks.Value-}
```
public final void addLookupValue(Value value)
```


向内部查找列表添加一个值。这是对 `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)) 进行操作的首选方式。

--------------------

&gt; ```
&gt; 使用此代码向查找列表添加新值：
&gt; ``````

taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Value](../../com.aspose.tasks/value) | Value to add into lookup.

--------------------

This method works only for [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instances which have `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup). |

### compareTo(ExtendedAttributeDefinition o) {#compareTo-com.aspose.tasks.ExtendedAttributeDefinition-}
```
public int compareTo(ExtendedAttributeDefinition o)
```


Compares this object with another instance of the @\{code ExtendedAttributeDefinition\} class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) | the object to be compared. |

**Returns:**
int - a negative integer, zero, or a positive integer as this object is less than, equal to, or greater than the specified object.
### createExtendedAttribute() {#createExtendedAttribute--}
```
public final ExtendedAttribute createExtendedAttribute()
```


Creates a new extended attribute with the field ID which equals to this object's field ID value.

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(boolean flagValue) {#createExtendedAttribute-boolean-}
```
public final ExtendedAttribute createExtendedAttribute(boolean flagValue)
```


Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified flag value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| flagValue | boolean | The specified flag value. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Duration durationValue) {#createExtendedAttribute-com.aspose.tasks.Duration-}
```
public final ExtendedAttribute createExtendedAttribute(Duration durationValue)
```


Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified duration value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | The specified duration value. |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Value lookupValue) {#createExtendedAttribute-com.aspose.tasks.Value-}
```
public final ExtendedAttribute createExtendedAttribute(Value lookupValue)
```


Creates new extended attribute linked with specified [Value](../../com.aspose.tasks/value) item.

--------------------

&gt; ```
&gt; Use this code to create new [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) using specific value:
&gt; ``````

 taskTextAttr.addLookupValue(value1);
 taskTextAttr.addLookupValue(value2);
 ExtendedAttribute extendedAttribute = taskTextAttr.createExtendedAttribute(value2);
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | lookupValue | [Value](../../com.aspose.tasks/value) | 指定的 [Value](../../com.aspose.tasks/value) 项。 |

--------------------

`lookupValue` 应该事先添加到 [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) 中，使用 [addLookupValue(Value)](../../com.aspose.tasks/extendedattributedefinition\#addLookupValue-Value-) 方法。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class linked with specified [Value](../../com.aspose.tasks/value) item.
### createExtendedAttribute(String textValue) {#createExtendedAttribute-java.lang.String-}
```
public final ExtendedAttribute createExtendedAttribute(String textValue)
```


创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的文本值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| textValue | java.lang.String | 指定的文本值。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(BigDecimal numericValue) {#createExtendedAttribute-java.math.BigDecimal-}
```
public final ExtendedAttribute createExtendedAttribute(BigDecimal numericValue)
```


创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的数值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| numericValue | java.math.BigDecimal | 指定的数值。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createExtendedAttribute(Date dateTimeValue) {#createExtendedAttribute-java.util.Date-}
```
public final ExtendedAttribute createExtendedAttribute(Date dateTimeValue)
```


创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的日期值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dateTimeValue | java.util.Date | 指定的日期时间值。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - returns created instance of the [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) class with the fieldID which equals to this object's fieldID value.
### createLookupResourceDefinition(int customFieldType, int fieldId, String alias) {#createLookupResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int customFieldType, int fieldId, String alias)
```


工厂方法用于创建带查找的扩展属性定义。它的 `CalculationType`（[getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)）等于 [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup)，且仅可在资源中使用。调用此方法时需要指定 `customFieldType`、`fieldId` 和 `alias`。

--------------------

&gt; ```
&gt; 使用此示例为具有查找的资源创建自定义字段定义，然后用文本值填充它：
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
resourceTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Text value 2");
this.setDescription("Text value description 2");
}});
project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createLookupResourceDefinition(int fieldId, String alias) {#createLookupResourceDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupResourceDefinition(int fieldId, String alias)
```


Factory method which creates an extended attribute definition with lookup. It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) and can be used in Resources only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom field definition for a resource with lookup and then fill it with text values:
&gt; ``````

 ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
     resourceTextAttr.addLookupValue(new Value() {{
         this.setId(1);
         this.setVal("Text value 1");
         this.setDescription("Text value description 1");
     }});
     resourceTextAttr.addLookupValue(new Value() {{
         this.setId(2);
         this.setVal("Text value 2");
         this.setDescription("Text value description 2");
     }});
     project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldId | int | 指定的 [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) 字段 ID。 |
| alias | java.lang.String | 指定的 String 别名。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createLookupTaskDefinition(int customFieldType, int fieldId, String alias) {#createLookupTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int customFieldType, int fieldId, String alias)
```


工厂方法，用于创建带查找的扩展属性定义。它的 `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\\#setCalculationType-int-)) 等于 [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\\#Lookup) 并且只能在任务中使用。调用此方法时需要指定 `customFieldType`、`fieldId` 和 `alias`。

--------------------

&gt; ```
&gt; 使用此示例为具有查找的任务创建自定义字段定义，然后用文本值填充它：
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, \"My custom field\");
taskTextAttr.addLookupValue(new Value() {{
this.setId(1);
this.setVal("Text value 1");
this.setDescription("Text value description 1");
}});
taskTextAttr.addLookupValue(new Value() {{
this.setId(2);
this.setVal("Text value 2");
this.setDescription("Text value description 2");
}});
project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createLookupTaskDefinition(int fieldId, String alias) {#createLookupTaskDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createLookupTaskDefinition(int fieldId, String alias)
```


Factory method which creates an extended attribute definition with lookup. It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup) and can be used in Tasks only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom field definition for a task with lookup and then fill it with text values:
&gt; ``````

 ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
 taskTextAttr.addLookupValue(new Value() {{
     this.setId(1);
     this.setVal("Text value 1");
     this.setDescription("Text value description 1");
 }});
 taskTextAttr.addLookupValue(new Value() {{
     this.setId(2);
     this.setVal("Text value 2");
     this.setDescription("Text value description 2");
 }});
 project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldId | int | 指定的 [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) 字段 ID。 |
| alias | java.lang.String | 指定的 String 别名。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createResourceDefinition(int customFieldType, int fieldId, String alias) {#createResourceDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int customFieldType, int fieldId, String alias)
```


工厂方法，用于创建简单的扩展属性定义，Microsoft Project 中显示为 “None”。它的 `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\\#setCalculationType-int-)) 等于 [CalculationType.None](../../com.aspose.tasks/calculationtype\\#None) 并且只能在资源中使用。调用此方法时需要指定 `customFieldType`、`fieldId` 和 `alias`。

--------------------

&gt; ```
&gt; 使用此示例创建自定义文本字段定义：
&gt; ``````

ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, \"My custom field\");
project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createResourceDefinition(int fieldId, String alias) {#createResourceDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createResourceDefinition(int fieldId, String alias)
```


Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) and can be used in Resource only. You are required to specify `fieldId` and `alias` when call this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom text field definition:
&gt; ``````

 ExtendedAttributeDefinition resourceTextAttr = ExtendedAttributeDefinition.createResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
 project.getExtendedAttributes().add(resourceTextAttr);
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldId | int | 指定的 [ExtendedAttributeResource](../../com.aspose.tasks/extendedattributeresource) 字段 ID。 |
| alias | java.lang.String | 指定的 String 别名。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### createTaskDefinition(int customFieldType, int fieldId, String alias) {#createTaskDefinition-int-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int customFieldType, int fieldId, String alias)
```


工厂方法，用于创建简单的扩展属性定义，Microsoft Project 中显示为 “None”。它的 `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\\#setCalculationType-int-)) 等于 [CalculationType.None](../../com.aspose.tasks/calculationtype\\#None) 并且只能在任务中使用。调用此方法时需要指定 `customFieldType`、`fieldId` 和 `alias`。

--------------------

&gt; ```
&gt; 使用此示例创建自定义文本字段定义：
&gt; ``````

ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, \"My custom field\");
project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | int | The specified [CustomFieldType](../../com.aspose.tasks/customfieldtype) type. |
| fieldId | int | The specified [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) field ID. |
| alias | java.lang.String | The specified String alias. |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `customFieldType`, `fieldId` and `alias`.
### createTaskDefinition(int fieldId, String alias) {#createTaskDefinition-int-java.lang.String-}
```
public static ExtendedAttributeDefinition createTaskDefinition(int fieldId, String alias)
```


Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has `CalculationType`([getCalculationType()](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType--)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.None](../../com.aspose.tasks/calculationtype\#None) and can be used in Tasks only. You are required to specify `fieldId` and `alias` when calling this method. The field type is inferred from field id.

--------------------

&gt; ```
&gt; Use this example to create a custom text field definition:
&gt; ``````

 ExtendedAttributeDefinition taskTextAttr = ExtendedAttributeDefinition.createTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
 project.getExtendedAttributes().add(taskTextAttr);
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldId | int | 指定的 [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) 字段 ID。 |
| alias | java.lang.String | 指定的 String 别名。 |

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - Created instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class with specified `fieldId` and `alias`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个标志，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 指定的用于与此实例比较的对象。 |

**Returns:**
boolean - 表示此实例是否等于指定对象的标志。
### getAlias() {#getAlias--}
```
public final String getAlias()
```


获取自定义字段的别名。

**Returns:**
java.lang.String - 自定义字段的别名。
### getAppendNewValues() {#getAppendNewValues--}
```
public final boolean getAppendNewValues()
```


获取一个值，指示添加到项目的新值是否会自动添加到列表中。

--------------------

当前支持 MSP 2003/2007 Xml 和 MSP 2003 mpp 格式。

**Returns:**
boolean - 表示添加到项目的新值是否自动加入列表的值。
### getAutoRollDown() {#getAutoRollDown--}
```
public final boolean getAutoRollDown()
```


获取一个值，指示是否已启用对任务分配的自动向下滚动。

**Returns:**
boolean - 表示是否启用自动向分配下放的值。
### getCalculationType() {#getCalculationType--}
```
public final int getCalculationType()
```


获取自定义属性值的计算类型。

**Returns:**
int - 自定义属性值的计算类型。
### getCfType() {#getCfType--}
```
public final int getCfType()
```


获取自定义字段的类型。

**Returns:**
int - 自定义字段的类型。
### getDefault() {#getDefault--}
```
public final String getDefault()
```


获取列表中的默认值。

--------------------

当前支持 MSP 2003/2007 Xml 和 MSP 2003 mpp 格式。

**Returns:**
java.lang.String - 列表中的默认值。
### getDefaultGuid() {#getDefaultGuid--}
```
public final String getDefaultGuid()
```


获取默认查找表条目的 Guid。

**Returns:**
java.lang.String - 默认查找表条目的 Guid。
### getElementType() {#getElementType--}
```
public final int getElementType()
```


获取扩展属性是否与任务、资源或分配关联。

**Returns:**
int - 扩展属性与任务、资源或分配关联。
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Gets 对应于自定义字段的项目 ID。使用来自 [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) 类的常量的字符串表示来指定 `FieldId`（[getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) 属性。

--------------------

&gt; ```
&gt;
&gt; ``````

customFieldDefinition.setFieldId(Integer.toString(ExtendedAttributeTask.Number10));
 
```

--------------------

Preferable way to set `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) property is to create [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) using one of the dedicated factory methods like [createTaskDefinition(int, String)](../../com.aspose.tasks/extendedattributedefinition\#createTaskDefinition-int--String-) or [createLookupTaskDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-).

**Returns:**
java.lang.String - corresponds to the project id of a custom field.
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


Gets the name of a custom field.

--------------------

Should not be set directly, instead create ExtendedAttributeDefinition using strongly typed static factory methods named like create\*Definition().

**Returns:**
java.lang.String - the name of a custom field.
### getFormula() {#getFormula--}
```
public final String getFormula()
```


Gets the formula that Microsoft Project uses to populate a custom task field.

**Returns:**
java.lang.String - the formula that Microsoft Project uses to populate a custom task field.
### getGraphicalIndicator() {#getGraphicalIndicator--}
```
public final GraphicalIndicatorsInfo getGraphicalIndicator()
```


Gets a graphical indicators info associated with the extended attribute. Applicable to MPP format.

**Returns:**
[GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) - a graphical indicators info associated with the extended attribute.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Gets the Guid of a custom field.

--------------------

Currently supported for Xml format only.

**Returns:**
java.lang.String - the Guid of a custom field.
### getLookupUid() {#getLookupUid--}
```
public final String getLookupUid()
```


Gets a Guid of the lookup table associated with a custom field.

--------------------

In order to create a custom field with lookup, use one of the factory methods: [createLookupTaskDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-) or [createLookupResourceDefinition(int, int, String)](../../com.aspose.tasks/extendedattributedefinition\#createLookupResourceDefinition-int--int--String-).

**Returns:**
java.lang.String - a Guid of the lookup table associated with a custom field.
### getMaxMultiValues() {#getMaxMultiValues--}
```
public final int getMaxMultiValues()
```


Gets the maximum number of values you can set in a pick list.

--------------------

Currently supported for Xml format only.

**Returns:**
int - the maximum number of values you can set in a pick list.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project for the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instance.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project for the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instance.
### getPhoneticsAlias() {#getPhoneticsAlias--}
```
public final String getPhoneticsAlias()
```


Gets the phonetic pronunciation of the alias of a custom field.

--------------------

Currently supported for Xml format only.

**Returns:**
java.lang.String - the phonetic pronunciation of the alias of a custom field.
### getRestrictValues() {#getRestrictValues--}
```
public final boolean getRestrictValues()
```


Gets a value indicating whether the custom field values are restricted to values in the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Returns:**
boolean - a value indicating whether the custom field values are restricted to values in the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).
### getRollupType() {#getRollupType--}
```
public final int getRollupType()
```


Gets the way rollups are calculated.

--------------------

Writing currently supported for Xml format only.

**Returns:**
int - the way rollups are calculated.
### getSecondaryGuid() {#getSecondaryGuid--}
```
public final String getSecondaryGuid()
```


Gets the secondary guid of extended attribute.

--------------------

This is new for MS Project 2010 property.

**Returns:**
java.lang.String - the secondary guid of extended attribute.
### getSecondaryPid() {#getSecondaryPid--}
```
public final String getSecondaryPid()
```


Gets the secondary PID of a custom field.

**Returns:**
java.lang.String - the secondary PID of a custom field.
### getSummaryRowsCalculationType() {#getSummaryRowsCalculationType--}
```
public final int getSummaryRowsCalculationType()
```


Gets the type of calculation of the custom attribute's value for summary rows.

**Returns:**
int - the type of calculation of the custom attribute's value for summary rows.
### getUserDef() {#getUserDef--}
```
public final boolean getUserDef()
```


Gets a value indicating whether a custom field is user defined.

--------------------

Currently supported for Xml format only.

**Returns:**
boolean - a value indicating whether a custom field is user defined.
### getValueList() {#getValueList--}
```
public final List<Value> getValueList()
```


Gets the List&lt;Value&gt; ValueList.

--------------------

When values of extended attributes are specified as properties of elements in the schema, they may either be specified by values or by references to the values contained in this list. Applications may assume ordering of the list by ordering specified here. Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats. Do not change this list directly. Use ExtendedAttributeDefinition.addLookupValue/removeLookupValue methods instead.

**Returns:**
java.util.List&lt;com.aspose.tasks.Value&gt; - the List&lt;Value&gt; ValueList.
### getValuelistSortOrder() {#getValuelistSortOrder--}
```
public final int getValuelistSortOrder()
```


Gets the way value lists are sorted. Values are: 0=Descending, 1=Ascending.

--------------------

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Returns:**
int - the way value lists are sorted.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code for the instance of the [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) class.

**Returns:**
int - a hash code for this object.
### removeLookupValue(Value value) {#removeLookupValue-com.aspose.tasks.Value-}
```
public final void removeLookupValue(Value value)
```


Removes a value from the internal lookup list. This is a preferable way for manipulations with the `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Value](../../com.aspose.tasks/value) | Value to remove from lookup.

--------------------

This method works only for [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) instances which have `CalculationType`([getCalculationType](../../com.aspose.tasks/extendedattributedefinition\#getCalculationType)/ [setCalculationType(int)](../../com.aspose.tasks/extendedattributedefinition\#setCalculationType-int-)) equals to [CalculationType.Lookup](../../com.aspose.tasks/calculationtype\#Lookup). |

### setAlias(String value) {#setAlias-java.lang.String-}
```
public final void setAlias(String value)
```


Sets the alias of a custom field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the alias of a custom field. |

### setAppendNewValues(boolean value) {#setAppendNewValues-boolean-}
```
public final void setAppendNewValues(boolean value)
```


Sets a value indicating whether new values added to a project are automatically added to the list.

--------------------

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether new values added to a project are automatically added to the list. |

### setAutoRollDown(boolean value) {#setAutoRollDown-boolean-}
```
public final void setAutoRollDown(boolean value)
```


Sets a value indicating whether an automatic roll down to assignments is enabled.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether an automatic roll down to assignments is enabled. |

### setCalculationType(int value) {#setCalculationType-int-}
```
public final void setCalculationType(int value)
```


Sets the type of calculation of the custom attribute's value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the type of calculation of the custom attribute's value. |

### setDefault(String value) {#setDefault-java.lang.String-}
```
public final void setDefault(String value)
```


Sets the default value in the list.

Currently supported for MSP 2003/2007 Xml and MSP 2003 mpp formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the default value in the list. |

### setDefaultGuid(String value) {#setDefaultGuid-java.lang.String-}
```
public final void setDefaultGuid(String value)
```


Sets the Guid of the default lookup table entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the Guid of the default lookup table entry. |

### setElementType(int value) {#setElementType-int-}
```
public final void setElementType(int value)
```


Sets the extended attribute is associated with a task, a resource or an assignment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the extended attribute is associated with a task, a resource or an assignment. |

### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Sets corresponds to the project id of a custom field. Use string representation of a constant from [ExtendedAttributeTask](../../com.aspose.tasks/extendedattributetask) class to specify `FieldId`([getFieldId()](../../com.aspose.tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose.tasks/extendedattributedefinition\#setFieldId-String-)) property.

--------------------

&gt; ```
&gt; 
&gt; ``````

 customFieldDefinition.setFieldId(Integer.toString(ExtendedAttributeTask.Number10));
 
```

--------------------

设置 `FieldId`([getFieldId()](../../com.aspose/tasks/extendedattributedefinition\#getFieldId--)/ [setFieldId(String)](../../com.aspose/tasks/extendedattributedefinition\#setFieldId-String-)) 属性的首选方式是创建 [ExtendedAttributeDefinition](../../com.aspose/tasks/extendedattributedefinition)，使用专用工厂方法之一，例如 [createTaskDefinition(int, String)](../../com.aspose/tasks/extendedattributedefinition\#createTaskDefinition-int--String-) 或 [createLookupTaskDefinition(int, int, String)](../../com.aspose/tasks/extendedattributedefinition\#createLookupTaskDefinition-int--int--String-)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 对应于自定义字段的项目 ID。 |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public final void setFormula(String value)
```


设置 Microsoft Project 用于填充自定义任务字段的公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | Microsoft Project 用于填充自定义任务字段的公式。 |

### setGraphicalIndicator(GraphicalIndicatorsInfo value) {#setGraphicalIndicator-com.aspose.tasks.GraphicalIndicatorsInfo-}
```
public final void setGraphicalIndicator(GraphicalIndicatorsInfo value)
```


设置与扩展属性关联的图形指示器信息。适用于 MPP 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GraphicalIndicatorsInfo](../../com.aspose.tasks/graphicalindicatorsinfo) | 与扩展属性关联的图形指示器信息。 |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


设置自定义字段的 Guid。

--------------------

目前仅支持 Xml 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 自定义字段的 Guid。 |

### setMaxMultiValues(int value) {#setMaxMultiValues-int-}
```
public final void setMaxMultiValues(int value)
```


设置在下拉列表中可以设置的最大值数量。

--------------------

目前仅支持 Xml 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在下拉列表中可以设置的最大值数量。 |

### setPhoneticsAlias(String value) {#setPhoneticsAlias-java.lang.String-}
```
public final void setPhoneticsAlias(String value)
```


设置自定义字段别名的拼音发音。

--------------------

目前仅支持 Xml 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 自定义字段别名的拼音发音。 |

### setRestrictValues(boolean value) {#setRestrictValues-boolean-}
```
public final void setRestrictValues(boolean value)
```


设置一个值，指示自定义字段的值是否受限于 `ValueList`([getValueList()](../../com.aspose.tasks/extendedattributedefinition\#getValueList--)/ [setValueList(List)](../../com.aspose.tasks/extendedattributedefinition\#setValueList-List-Value--))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个指示自定义字段值是否受限于该 |

### setRollupType(int value) {#setRollupType-int-}
```
public final void setRollupType(int value)
```


设置汇总的计算方式。

--------------------

写入目前仅支持 Xml 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 汇总的计算方式。 |

### setSecondaryGuid(String value) {#setSecondaryGuid-java.lang.String-}
```
public final void setSecondaryGuid(String value)
```


设置扩展属性的次要 guid。

--------------------

这是 MS Project 2010 的新属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 扩展属性的次要 guid。 |

### setSecondaryPid(String value) {#setSecondaryPid-java.lang.String-}
```
public final void setSecondaryPid(String value)
```


设置自定义字段的次要 PID。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | 自定义字段的次要 PID。 |

### setSummaryRowsCalculationType(int value) {#setSummaryRowsCalculationType-int-}
```
public final void setSummaryRowsCalculationType(int value)
```


设置汇总行中自定义属性值的计算类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 汇总行中自定义属性值的计算类型。 |

### setUserDef(boolean value) {#setUserDef-boolean-}
```
public final void setUserDef(boolean value)
```


设置一个值，指示自定义字段是否为用户定义。

--------------------

目前仅支持 Xml 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个指示自定义字段是否为用户定义的值。 |

### setValuelistSortOrder(int value) {#setValuelistSortOrder-int-}
```
public final void setValuelistSortOrder(int value)
```


设置值列表的排序方式。取值为：0=降序，1=升序。

--------------------

当前支持 MSP 2003/2007 Xml 和 MSP 2003 mpp 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 值列表的排序方式。 |

