---
title: Baseline
second_title: Aspose.Tasks for Java API Reference
description: Represents baseline values of a resource.
type: docs
weight: 26
url: /java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Represents baseline values of a resource.
## Constructors

| Constructor | Description |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Methods

| Method | Description |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | IComparable interface implementation. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Returns a value indicating whether this instance is equal to a specified object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [getBaselineNumber()](#getBaselineNumber--) | Gets the unique number of a baseline data record. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Sets the unique number of a baseline data record. |
| [getBcwp()](#getBcwp--) | Gets the budgeted cost of a work performed by a resource for a project to-date. |
| [setBcwp(double value)](#setBcwp-double-) | Sets the budgeted cost of a work performed by a resource for a project to-date. |
| [getBcws()](#getBcws--) | Gets the budget cost of a work scheduled for a resource. |
| [setBcws(double value)](#setBcws-double-) | Sets the budget cost of a work scheduled for a resource. |
| [getCost()](#getCost--) | Gets the projected cost of a resource when the baseline is saved. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Sets the projected cost of a resource when the baseline is saved. |
| [getWork()](#getWork--) | Gets the work assigned to a resource when the baseline is saved. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Sets the work assigned to a resource when the baseline is saved. |
| [hashCode()](#hashCode--) | Returns a hash code value for the baseline. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returns a value indicating whether this instance is equal to a specified object. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returns a value indicating whether this instance is greater than a specified object. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returns a value indicating whether this instance is greater than or equal to a specified object. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returns a value indicating whether this instance is not equal to a specified object. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returns a value indicating whether this instance is less than a specified object. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returns a value indicating whether this instance is less than or equal to a specified object. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


IComparable interface implementation. Compares this instance to the specified Baseline object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | the specified Baseline object to compare this instance to. |

**Returns:**
int - returns -1 if this instance is less than the specified object, 1 if this instance is greater than the specified object; otherwise returns 0
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | the specified object to compare with this instance. |

**Returns:**
boolean - returns true if this instance is equal to the specified object; otherwise, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | the specified object to compare with this instance. |

**Returns:**
boolean - returns true if this instance is equal to the specified object; otherwise, false.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Gets the unique number of a baseline data record.

**Returns:**
int - the unique number of a baseline data record.
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Sets the unique number of a baseline data record.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the unique number of a baseline data record. |

### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Gets the budgeted cost of a work performed by a resource for a project to-date.

**Returns:**
double - the budgeted cost of a work performed by a resource for a project to-date.
### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Sets the budgeted cost of a work performed by a resource for a project to-date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | the budgeted cost of a work performed by a resource for a project to-date. |

### getBcws() {#getBcws--}
```
public final double getBcws()
```


Gets the budget cost of a work scheduled for a resource.

**Returns:**
double - the budget cost of a work scheduled for a resource.
### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Sets the budget cost of a work scheduled for a resource.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | the budget cost of a work scheduled for a resource. |

### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Gets the projected cost of a resource when the baseline is saved.

**Returns:**
java.math.BigDecimal - the projected cost of a resource when the baseline is saved.
### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Sets the projected cost of a resource when the baseline is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.math.BigDecimal | the projected cost of a resource when the baseline is saved. |

### getWork() {#getWork--}
```
public final Duration getWork()
```


Gets the work assigned to a resource when the baseline is saved.

Value: The amount of assigned work to a resource when the baseline was saved.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Sets the work assigned to a resource when the baseline is saved.

Value: The amount of assigned work to a resource when the baseline was saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | the work assigned to a resource when the baseline is saved. |

### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for the baseline.

**Returns:**
int - returns a hash code value for this object.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | The first baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | The second baseline. |

**Returns:**
boolean - a value indicating whether this instance is equal to a specified object
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Returns a value indicating whether this instance is greater than a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | The first baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | The second baseline. |

**Returns:**
boolean - a value indicating whether this instance is greater than a specified object
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Returns a value indicating whether this instance is greater than or equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | The first baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | The second baseline. |

**Returns:**
boolean - a value indicating whether this instance is greater than or equal to a specified object
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Returns a value indicating whether this instance is not equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | The first baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | The second baseline. |

**Returns:**
boolean - a value indicating whether this instance is not equal to a specified object
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Returns a value indicating whether this instance is less than a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | The first baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | The second baseline. |

**Returns:**
boolean - a value indicating whether this instance is less than a specified object
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Returns a value indicating whether this instance is less than or equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | The first baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | The second baseline. |

**Returns:**
boolean - a value indicating whether this instance is less than or equal to a specified object
