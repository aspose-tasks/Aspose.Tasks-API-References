---
title: RiskItemStatistics
second_title: Aspose.Tasks for Java API Reference
description: Represents an item which stores statistical data for the task of the analyzed project.
type: docs
weight: 264
url: /java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Represents an item which stores statistical data for the task of the analyzed project.
## Methods

| Method | Description |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Gets the expected value of the risk item. |
| [getItemType()](#getItemType--) | Gets an instance of the [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeration. |
| [getMaximum()](#getMaximum--) | Gets the maximum value which was generated during Monte Carlo simulation. |
| [getMinimum()](#getMinimum--) | Gets the minimum value which was generated during Monte Carlo simulation. |
| [getPercentile(int percent)](#getPercentile-int-) | Gets a value below which a specified percentage of generated samples fall. |
| [getStandardDeviation()](#getStandardDeviation--) | Gets the standard deviation of the risk item. |
| [toString()](#toString--) | Returns short string representation of a risk item. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Gets the expected value of the risk item.

**Returns:**
java.util.Date - the expected value of the risk item.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Gets an instance of the [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeration.

**Returns:**
int - an instance of the [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeration.
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Gets the maximum value which was generated during Monte Carlo simulation.

**Returns:**
java.util.Date - the maximum value which was generated during Monte Carlo simulation.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Gets the minimum value which was generated during Monte Carlo simulation.

**Returns:**
java.util.Date - the minimum value which was generated during Monte Carlo simulation.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Gets a value below which a specified percentage of generated samples fall.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| percent | int | the specified percent between 0 and 100. |

**Returns:**
java.util.Date - a value below which a specified percentage of generated samples fall.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Gets the standard deviation of the risk item.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Returns short string representation of a risk item. The exact details of the representation are unspecified and subject to change.

**Returns:**
java.lang.String - short string which represents RiskItem object.
