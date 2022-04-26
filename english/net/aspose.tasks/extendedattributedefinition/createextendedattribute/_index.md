---
title: CreateExtendedAttribute
second_title: Aspose.Tasks for .NET API Reference
description: 
type: docs
weight: 300
url: /net/aspose.tasks/extendedattributedefinition/createextendedattribute/
---
## ExtendedAttributeDefinition.CreateExtendedAttribute method (1 of 7)

Creates a new extended attribute with the field ID which equals to this object's field ID value.

```csharp
public ExtendedAttribute CreateExtendedAttribute()
```

## Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute) class with the fieldID which equals to this object's fieldID value.

### See Also

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* namespace [Aspose.Tasks](../../extendedattributedefinition)
* assembly [Aspose.Tasks](../../../)

---

## ExtendedAttributeDefinition.CreateExtendedAttribute method (2 of 7)

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified text value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(string textValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| textValue | String | The specified text value. |

## Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype) is not 'Text' |

### See Also

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* namespace [Aspose.Tasks](../../extendedattributedefinition)
* assembly [Aspose.Tasks](../../../)

---

## ExtendedAttributeDefinition.CreateExtendedAttribute method (3 of 7)

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified numeric value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(decimal numericValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| numericValue | Decimal | The specified numeric value. |

## Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype) is not 'Number' or 'Cost' |

### See Also

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* namespace [Aspose.Tasks](../../extendedattributedefinition)
* assembly [Aspose.Tasks](../../../)

---

## ExtendedAttributeDefinition.CreateExtendedAttribute method (4 of 7)

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified date value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(DateTime dateTimeValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dateTimeValue | DateTime | The specified date time value. |

## Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype) is not 'Date', 'Start' or 'Finish' |

### See Also

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* namespace [Aspose.Tasks](../../extendedattributedefinition)
* assembly [Aspose.Tasks](../../../)

---

## ExtendedAttributeDefinition.CreateExtendedAttribute method (5 of 7)

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified duration value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Duration durationValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| durationValue | Duration | The specified duration value. |

## Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype) is not 'Duration' |

### See Also

* class [ExtendedAttribute](../../extendedattribute)
* struct [Duration](../../duration)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* namespace [Aspose.Tasks](../../extendedattributedefinition)
* assembly [Aspose.Tasks](../../../)

---

## ExtendedAttributeDefinition.CreateExtendedAttribute method (6 of 7)

Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified flag value.

```csharp
public ExtendedAttribute CreateExtendedAttribute(bool flagValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| flagValue | Boolean | The specified flag value. |

## Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute) class with the fieldID which equals to this object's fieldID value.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | If current [`CfType`](../cftype) is not 'Flag' |

### See Also

* class [ExtendedAttribute](../../extendedattribute)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* namespace [Aspose.Tasks](../../extendedattributedefinition)
* assembly [Aspose.Tasks](../../../)

---

## ExtendedAttributeDefinition.CreateExtendedAttribute method (7 of 7)

Creates new extended attribute linked with specified [`Value`](../../value) item.

```csharp
public ExtendedAttribute CreateExtendedAttribute(Value lookupValue)
```

| Parameter | Type | Description |
| --- | --- | --- |
| lookupValue | Value | The specified [`Value`](../../value) item. |

## Return Value

returns created instance of the [`ExtendedAttribute`](../../extendedattribute) class linked with specified [`Value`](../../value) item.

### Remarks

*lookupValue* should be previously added to the [`ExtendedAttributeDefinition`](../../extendedattributedefinition) using [`AddLookupValue`](../addlookupvalue) method.

### Examples

Use this code to create new [`ExtendedAttribute`](../../extendedattribute) using specific value:

```csharp
taskTextAttr.AddLookupValue(value1);
taskTextAttr.AddLookupValue(value2);
var extendedAttribute = taskTextAttr.CreateExtendedAttribute(value2);
```

### See Also

* class [ExtendedAttribute](../../extendedattribute)
* class [Value](../../value)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* namespace [Aspose.Tasks](../../extendedattributedefinition)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
