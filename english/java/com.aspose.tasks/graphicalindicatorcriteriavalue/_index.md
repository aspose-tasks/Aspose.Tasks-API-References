---
title: GraphicalIndicatorCriteriaValue
second_title: Aspose.Tasks for Java API Reference
description: Represents a value used in condition check of graphical indicators criteria.
type: docs
weight: 116
url: /java/com.aspose.tasks/graphicalindicatorcriteriavalue/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteriaValue
```

Represents a value used in condition check of graphical indicators criteria.
## Constructors

| Constructor | Description |
| --- | --- |
| [GraphicalIndicatorCriteriaValue(BigDecimal value)](#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-) | Creates an instance of GraphicalIndicatorCriteriaValue class with constant BigDecimal value. |
| [GraphicalIndicatorCriteriaValue(Date dateValue)](#GraphicalIndicatorCriteriaValue-java.util.Date-) | Creates an instance of GraphicalIndicatorCriteriaValue class with constant Date value. |
| [GraphicalIndicatorCriteriaValue(String textValue)](#GraphicalIndicatorCriteriaValue-java.lang.String-) | Creates an instance of GraphicalIndicatorCriteriaValue class with constant String value. |
| [GraphicalIndicatorCriteriaValue(Duration durationValue)](#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-) | Creates an instance of GraphicalIndicatorCriteriaValue class with constant Duration value. |
| [GraphicalIndicatorCriteriaValue(boolean flagValue)](#GraphicalIndicatorCriteriaValue-boolean-) | Creates an instance of GraphicalIndicatorCriteriaValue class with constant flag (boolean) value. |
## Methods

| Method | Description |
| --- | --- |
| [createFieldLink(int field)](#createFieldLink-int-) | Creates an instance of GraphicalIndicatorCriteriaValue class representing the value of the specified MS Project's field. |
| [getRawValue()](#getRawValue--) | Gets the underlying constant of Field value. |
| [isFieldLink()](#isFieldLink--) | Gets whether the current instance is a field link (represents a value of a field). |
| [toString()](#toString--) | Returns a string that represents the current object. |
### GraphicalIndicatorCriteriaValue(BigDecimal value) {#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-}
```
public GraphicalIndicatorCriteriaValue(BigDecimal value)
```


Creates an instance of GraphicalIndicatorCriteriaValue class with constant BigDecimal value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | the BigDecimal value |

### GraphicalIndicatorCriteriaValue(Date dateValue) {#GraphicalIndicatorCriteriaValue-java.util.Date-}
```
public GraphicalIndicatorCriteriaValue(Date dateValue)
```


Creates an instance of GraphicalIndicatorCriteriaValue class with constant Date value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dateValue | java.util.Date | the Date value |

### GraphicalIndicatorCriteriaValue(String textValue) {#GraphicalIndicatorCriteriaValue-java.lang.String-}
```
public GraphicalIndicatorCriteriaValue(String textValue)
```


Creates an instance of GraphicalIndicatorCriteriaValue class with constant String value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| textValue | java.lang.String | the String value |

### GraphicalIndicatorCriteriaValue(Duration durationValue) {#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-}
```
public GraphicalIndicatorCriteriaValue(Duration durationValue)
```


Creates an instance of GraphicalIndicatorCriteriaValue class with constant Duration value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | the Duration value |

### GraphicalIndicatorCriteriaValue(boolean flagValue) {#GraphicalIndicatorCriteriaValue-boolean-}
```
public GraphicalIndicatorCriteriaValue(boolean flagValue)
```


Creates an instance of GraphicalIndicatorCriteriaValue class with constant flag (boolean) value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| flagValue | boolean | the flag (boolean) value |

### createFieldLink(int field) {#createFieldLink-int-}
```
public static GraphicalIndicatorCriteriaValue createFieldLink(int field)
```


Creates an instance of GraphicalIndicatorCriteriaValue class representing the value of the specified MS Project's field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| field | int | the specified field |

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - instance of GraphicalIndicatorCriteriaValue class representing the value of the specified field
### getRawValue() {#getRawValue--}
```
public final Object getRawValue()
```


Gets the underlying constant of Field value.

**Returns:**
java.lang.Object - the underlying constant of Field value
### isFieldLink() {#isFieldLink--}
```
public final boolean isFieldLink()
```


Gets whether the current instance is a field link (represents a value of a field).

**Returns:**
boolean - whether the current instance is a field link (represents a value of a field)
### toString() {#toString--}
```
public String toString()
```


Returns a string that represents the current object.

**Returns:**
java.lang.String - a string that represents the current object
