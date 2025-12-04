---
title: TimescaleTier
second_title: Aspose.Tasks for Java API Reference
description: Represents a single tier of the timescale on a Gantt Chart.
type: docs
weight: 322
url: /java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Represents a single tier of the timescale on a Gantt Chart.
## Constructors

| Constructor | Description |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | Initializes a new instance of the [TimescaleTier](../../com.aspose.tasks/timescaletier) class. |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | Initializes a new instance of the [TimescaleTier](../../com.aspose.tasks/timescaletier) class. |
## Methods

| Method | Description |
| --- | --- |
| [getAlignment()](#getAlignment--) | Gets how to align labels within each time period of the tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | Gets the time unit interval in which to show labels for the tier. |
| [getDateTimeConverter()](#getDateTimeConverter--) | Gets a callback function for handling rendering date tick in this tier. |
| [getLabel()](#getLabel--) | Gets date label [DateLabel](../../com.aspose.tasks/datelabel) for the timescale tier. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | Gets flag that defines whether date labels should be rendered on each page when a time period spans over several pages. |
| [getShowTicks()](#getShowTicks--) | Gets a value indicating whether whether to show tick marks that separate time periods in the tier. |
| [getUnit()](#getUnit--) | Gets timescale unit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) for the timescale tier. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | Gets a value indicating whether to base the tier labels on the fiscal year. |
| [setAlignment(int value)](#setAlignment-int-) | Sets how to align labels within each time period of the tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | Sets the time unit interval in which to show labels for the tier. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | Sets a callback function for handling rendering date tick in this tier. |
| [setLabel(int value)](#setLabel-int-) | Sets date label [DateLabel](../../com.aspose.tasks/datelabel) for the timescale tier. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | Sets flag that defines whether date labels should be rendered on each page when a time period spans over several pages. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | Sets a value indicating whether whether to show tick marks that separate time periods in the tier. |
| [setUnit(int value)](#setUnit-int-) | Sets timescale unit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) for the timescale tier. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | Sets a value indicating whether to base the tier labels on the fiscal year. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


Initializes a new instance of the [TimescaleTier](../../com.aspose.tasks/timescaletier) class.

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


Initializes a new instance of the [TimescaleTier](../../com.aspose.tasks/timescaletier) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| unit | int | The timescale unit [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | The count of [TimescaleUnit](../../com.aspose.tasks/timescaleunit) units. |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


Gets how to align labels within each time period of the tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - how to align labels within each time period of the tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


Gets the time unit interval in which to show labels for the tier. The default value is 1.

**Returns:**
int - the time unit interval in which to show labels for the tier.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


Gets a callback function for handling rendering date tick in this tier.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


Gets date label [DateLabel](../../com.aspose.tasks/datelabel) for the timescale tier.

**Returns:**
int - date label [DateLabel](../../com.aspose.tasks/datelabel) for the timescale tier.
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


Gets flag that defines whether date labels should be rendered on each page when a time period spans over several pages. If value is 'true', when time period spans over several pages, date labels for the period are rendered on each page. If values is 'false', date label is rendered only once according to a value of `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) property.

--------------------

Doesn't have the equivalent in MS Project.

**Returns:**
boolean - flag that defines whether date labels should be rendered on each page when a time period spans over several pages.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


Gets a value indicating whether whether to show tick marks that separate time periods in the tier.

**Returns:**
boolean - a value indicating whether whether to show tick marks that separate time periods in the tier.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


Gets timescale unit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) for the timescale tier. The default value is [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Returns:**
int - timescale unit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) for the timescale tier.
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


Gets a value indicating whether to base the tier labels on the fiscal year.

**Returns:**
boolean - a value indicating whether to base the tier labels on the fiscal year.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


Sets how to align labels within each time period of the tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | how to align labels within each time period of the tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


Sets the time unit interval in which to show labels for the tier. The default value is 1.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the time unit interval in which to show labels for the tier. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


Sets a callback function for handling rendering date tick in this tier.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | a callback function for handling rendering date tick in this tier. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


Sets date label [DateLabel](../../com.aspose.tasks/datelabel) for the timescale tier.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | date label [DateLabel](../../com.aspose.tasks/datelabel) for the timescale tier. |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


Sets flag that defines whether date labels should be rendered on each page when a time period spans over several pages. If value is 'true', when time period spans over several pages, date labels for the period are rendered on each page. If values is 'false', date label is rendered only once according to a value of `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) property.

--------------------

Doesn't have the equivalent in MS Project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | flag that defines whether date labels should be rendered on each page when a time period spans over several pages. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


Sets a value indicating whether whether to show tick marks that separate time periods in the tier.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether whether to show tick marks that separate time periods in the tier. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


Sets timescale unit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) for the timescale tier. The default value is [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | timescale unit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) for the timescale tier. |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


Sets a value indicating whether to base the tier labels on the fiscal year.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to base the tier labels on the fiscal year. |

