---
title: "TimescaleTier"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine einzelne Ebene der Zeitskala in einem Gantt-Diagramm dar."
type: docs
weight: 325
url: /de/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Stellt eine einzelne Ebene der Zeitskala in einem Gantt-Diagramm dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | Initialisiert eine neue Instanz der Klasse [TimescaleTier](../../com.aspose.tasks/timescaletier). |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | Initialisiert eine neue Instanz der Klasse [TimescaleTier](../../com.aspose.tasks/timescaletier). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getAlignment()](#getAlignment--) | Ermittelt, wie Beschriftungen innerhalb jedes Zeitabschnitts der Ebene ausgerichtet werden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | Ermittelt das Zeitintervall, in dem Beschriftungen für die Ebene angezeigt werden. |
| [getDateTimeConverter()](#getDateTimeConverter--) | Ermittelt eine Callback-Funktion zur Behandlung der Darstellung von Datums-Ticks in dieser Ebene. |
| [getLabel()](#getLabel--) | Ermittelt das Datumslabel [DateLabel](../../com.aspose.tasks/datelabel) für die Zeitskalaebene. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | Ermittelt das Flag, das definiert, ob Datumsbeschriftungen auf jeder Seite gerendert werden sollen, wenn ein Zeitabschnitt sich über mehrere Seiten erstreckt. |
| [getShowTicks()](#getShowTicks--) | Ermittelt einen Wert, der angibt, ob Trennstriche, die Zeitabschnitte in der Ebene trennen, angezeigt werden sollen. |
| [getUnit()](#getUnit--) | Ermittelt die Zeitskalaeinheit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) für die Zeitskalaebene. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | Ermittelt einen Wert, der angibt, ob die Ebenenbeschriftungen auf dem Geschäftsjahr basieren sollen. |
| [setAlignment(int value)](#setAlignment-int-) | Legt fest, wie Beschriftungen innerhalb jedes Zeitabschnitts der Ebene ausgerichtet werden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | Legt das Zeitintervall fest, in dem Beschriftungen für die Ebene angezeigt werden. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | Legt eine Callback-Funktion fest, die die Darstellung von Datums-Ticks in dieser Ebene behandelt. |
| [setLabel(int value)](#setLabel-int-) | Legt das Datumslabel [DateLabel](../../com.aspose.tasks/datelabel) für die Zeitskalaebene fest. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | Legt das Flag fest, das definiert, ob Datumsbeschriftungen auf jeder Seite gerendert werden sollen, wenn ein Zeitabschnitt sich über mehrere Seiten erstreckt. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | Legt einen Wert fest, der angibt, ob Trennstriche, die Zeitabschnitte in der Ebene trennen, angezeigt werden sollen. |
| [setUnit(int value)](#setUnit-int-) | Legt die Zeitskalaeinheit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) für die Zeitskalaebene fest. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | Legt einen Wert fest, der angibt, ob die Ebenenbeschriftungen auf dem Geschäftsjahr basieren sollen. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


Initialisiert eine neue Instanz der Klasse [TimescaleTier](../../com.aspose.tasks/timescaletier).

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


Initialisiert eine neue Instanz der Klasse [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| unit | int | Die Zeitskalaeinheit [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | Die Anzahl der [TimescaleUnit](../../com.aspose.tasks/timescaleunit)-Einheiten. |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


Ermittelt, wie Beschriftungen innerhalb jedes Zeitabschnitts der Ebene ausgerichtet werden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - wie Beschriftungen innerhalb jedes Zeitabschnitts der Ebene ausgerichtet werden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


Ermittelt das Zeitintervall, in dem Beschriftungen für die Ebene angezeigt werden. Der Standardwert ist 1.

**Returns:**
int - das Zeitintervall, in dem Beschriftungen für die Ebene angezeigt werden.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


Ermittelt eine Callback-Funktion zur Behandlung der Darstellung von Datums-Ticks in dieser Ebene.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


Ermittelt das Datumslabel [DateLabel](../../com.aspose.tasks/datelabel) für die Zeitskalaebene.

**Returns:**
int - Datumslabel [DateLabel](../../com.aspose.tasks/datelabel) für die Zeitskalaebene.
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


Liest das Flag, das definiert, ob Datumsbeschriftungen auf jeder Seite gerendert werden sollen, wenn ein Zeitraum sich über mehrere Seiten erstreckt. Wenn der Wert 'true' ist, werden bei einem über mehrere Seiten erstreckenden Zeitraum die Datumsbeschriftungen für den Zeitraum auf jeder Seite gerendert. Wenn der Wert 'false' ist, wird die Datumsbeschriftung nur einmal gemäß dem Wert der `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) Eigenschaft.

--------------------

Hat keine Entsprechung in MS Project.

**Returns:**
boolean - Flag, das definiert, ob Datumsbeschriftungen auf jeder Seite gerendert werden sollen, wenn ein Zeitraum sich über mehrere Seiten erstreckt.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


Ermittelt einen Wert, der angibt, ob Trennstriche, die Zeitabschnitte in der Ebene trennen, angezeigt werden sollen.

**Returns:**
boolean - ein Wert, der angibt, ob Trennstriche angezeigt werden sollen, die Zeiträume in der Ebene voneinander trennen.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


Liest die Zeitskalaeinheit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) für die Zeitskalaebene. Der Standardwert ist [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Returns:**
int - Zeitskalaeinheit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) für die Zeitskalaebene.
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


Ermittelt einen Wert, der angibt, ob die Ebenenbeschriftungen auf dem Geschäftsjahr basieren sollen.

**Returns:**
boolean - ein Wert, der angibt, ob die Ebenenbeschriftungen auf dem Geschäftsjahr basieren sollen.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


Legt fest, wie Beschriftungen innerhalb jedes Zeitabschnitts der Ebene ausgerichtet werden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | int | wie Beschriftungen innerhalb jedes Zeitraums der Ebene ausgerichtet werden ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


Legt das Zeitintervall fest, in dem Beschriftungen für die Ebene angezeigt werden. Der Standardwert ist 1.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | das Zeitintervall, in dem Beschriftungen für die Ebene angezeigt werden. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


Legt eine Callback-Funktion fest, die die Darstellung von Datums-Ticks in dieser Ebene behandelt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | eine Callback-Funktion zur Behandlung des Renderns von Datumsstrichen in dieser Ebene. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


Legt das Datumslabel [DateLabel](../../com.aspose.tasks/datelabel) für die Zeitskalaebene fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | int | Datumsbeschriftung [DateLabel](../../com.aspose.tasks/datelabel) für die Zeitskalaebene. |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


Setzt das Flag, das definiert, ob Datumsbeschriftungen auf jeder Seite gerendert werden sollen, wenn ein Zeitraum sich über mehrere Seiten erstreckt. Wenn der Wert 'true' ist, werden bei einem über mehrere Seiten erstreckenden Zeitraum die Datumsbeschriftungen für den Zeitraum auf jeder Seite gerendert. Wenn der Wert 'false' ist, wird die Datumsbeschriftung nur einmal gemäß dem Wert der `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) Eigenschaft gerendert.

--------------------

Hat keine Entsprechung in MS Project.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Flag, das definiert, ob Datumsbeschriftungen auf jeder Seite gerendert werden sollen, wenn ein Zeitraum sich über mehrere Seiten erstreckt. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


Legt einen Wert fest, der angibt, ob Trennstriche, die Zeitabschnitte in der Ebene trennen, angezeigt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Trennstriche angezeigt werden sollen, die Zeiträume in der Ebene voneinander trennen. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


Setzt die Zeitskalaeinheit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) für die Zeitskalaebene. Der Standardwert ist [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | int | Zeitskalaeinheit [TimescaleUnit](../../com.aspose.tasks/timescaleunit) für die Zeitskalaebene. |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


Legt einen Wert fest, der angibt, ob die Ebenenbeschriftungen auf dem Geschäftsjahr basieren sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Ebenenbeschriftungen auf dem Geschäftsjahr basieren sollen. |

