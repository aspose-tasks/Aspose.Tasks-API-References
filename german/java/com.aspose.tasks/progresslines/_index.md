---
title: "ProgressLines"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt Fortschrittslinien in einer Gantt-Diagrammansicht dar."
type: docs
weight: 219
url: /de/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

Stellt Fortschrittslinien in einer Gantt-Diagrammansicht dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | Ermittelt das Datum, ab dem Fortschrittslinien angezeigt werden. |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | Ermittelt einen Wert, der angibt, ob Fortschrittslinien ab dem Beginn des Projektstartdatums angezeigt werden sollen. |
| [getDateFormat()](#getDateFormat--) | Ermittelt das Datumsformat ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | Ermittelt einen Wert, der angibt, ob die Fortschrittslinie am aktuellen Datum angezeigt wird. |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | Ermittelt einen Wert, der angibt, ob die Fortschrittslinie in wiederkehrenden Intervallen angezeigt wird. |
| [getDisplaySelected()](#getDisplaySelected--) | Ermittelt einen Wert, der angibt, ob Fortschrittslinien an den ausgewählten Daten angezeigt werden. |
| [getFont()](#getFont--) | Ermittelt die für das Fortschrittslinien-Label verwendete Schriftart. |
| [getLineColor()](#getLineColor--) | Ermittelt die Linienfarbe für die aktuelle Fortschrittslinie. |
| [getLinePattern()](#getLinePattern--) | Ermittelt das Linienmuster der aktuellen Fortschrittslinie. |
| [getOtherLineColor()](#getOtherLineColor--) | Ermittelt die Farbe der anderen Fortschrittslinie. |
| [getOtherLinePattern()](#getOtherLinePattern--) | Ermittelt das Linienmuster für die andere Fortschrittslinie. |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | Ermittelt die Farbe des anderen Fortschrittspunkts. |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | Ermittelt die Form des Fortschrittspunkts der anderen Fortschrittslinie. |
| [getProgressPointColor()](#getProgressPointColor--) | Ermittelt die Farbe des Fortschrittspunkts. |
| [getProgressPointShape()](#getProgressPointShape--) | Ermittelt die Form des Fortschrittspunkts. |
| [getRecurringInterval()](#getRecurringInterval--) | Ermittelt das wiederkehrende Intervall. |
| [getSelectedDates()](#getSelectedDates--) | Ermittelt die Liste der ausgewählten Daten, für die Fortschrittslinien angezeigt werden sollen. |
| [getShowDate()](#getShowDate--) | Ermittelt einen Wert, der angibt, ob das Datum für jede Fortschrittslinie angezeigt werden soll. |
| [isBaselinePlan()](#isBaselinePlan--) | Ermittelt einen Wert, der angibt, ob Fortschrittslinien für den Basisplan oder den Ist-Stand angezeigt werden sollen. |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | Legt einen Wert fest, der angibt, ob Fortschrittslinien für den Basisplan oder den Ist-Stand angezeigt werden sollen. |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | Legt das Datum fest, ab dem Fortschrittslinien angezeigt werden. |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | Legt einen Wert fest, der angibt, ob Fortschrittslinien ab dem Beginn des Projektstartdatums angezeigt werden sollen. |
| [setDateFormat(int value)](#setDateFormat-int-) | Legt das Datumsformat fest ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | Legt einen Wert fest, der angibt, ob die Fortschrittslinie am aktuellen Datum angezeigt werden soll. |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | Legt einen Wert fest, der angibt, ob die Fortschrittslinie in wiederkehrenden Intervallen angezeigt werden soll. |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | Legt einen Wert fest, der angibt, ob die Fortschrittslinien an den ausgewählten Daten angezeigt werden sollen. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Legt die für das Fortschrittslinien-Label verwendete Schriftart fest. |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | Legt die Linienfarbe für die aktuelle Fortschrittslinie fest. |
| [setLinePattern(int value)](#setLinePattern-int-) | Legt das Linienmuster der aktuellen Fortschrittslinie fest. |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | Legt die Farbe der anderen Fortschrittslinie fest. |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | Legt das Linienmuster für die andere Fortschrittslinie fest. |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | Legt die Farbe des anderen Fortschrittspunkts fest. |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | Legt die Form des Fortschrittspunkts der anderen Fortschrittslinie fest. |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | Legt die Farbe des Fortschrittspunkts fest. |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | Legt die Form des Fortschrittspunkts fest. |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | Legt das wiederkehrende Intervall fest. |
| [setShowDate(boolean value)](#setShowDate-boolean-) | Legt einen Wert fest, der angibt, ob das Datum für jede Fortschrittslinie angezeigt werden soll. |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


Ermittelt das Datum, ab dem Fortschrittslinien angezeigt werden.

**Returns:**
java.util.Date - das Datum, ab dem Fortschrittslinien angezeigt werden sollen.
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


Ermittelt einen Wert, der angibt, ob Fortschrittslinien ab dem Beginn des Projektstartdatums angezeigt werden sollen.

**Returns:**
boolean - ein Wert, der angibt, ob Fortschrittslinien ab dem Beginn des Projektstartdatums angezeigt werden sollen.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Ermittelt das Datumsformat ([DateLabel](../../com.aspose.tasks/datelabel)).

**Returns:**
int - das Datumsformat ([DateLabel](../../com.aspose.tasks/datelabel)).
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


Ermittelt einen Wert, der angibt, ob die Fortschrittslinie am aktuellen Datum angezeigt wird.

**Returns:**
boolean - ein Wert, der angibt, ob die Fortschrittslinie am aktuellen Datum angezeigt wird.
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


Ermittelt einen Wert, der angibt, ob die Fortschrittslinie in wiederkehrenden Intervallen angezeigt wird.

**Returns:**
boolean - ein Wert, der angibt, ob die Fortschrittslinie in wiederkehrenden Intervallen angezeigt wird.
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


Ermittelt einen Wert, der angibt, ob Fortschrittslinien an den ausgewählten Daten angezeigt werden.

**Returns:**
boolean - ein Wert, der angibt, ob Fortschrittslinien an den ausgewählten Daten angezeigt werden.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Ermittelt die für das Fortschrittslinien-Label verwendete Schriftart.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


Ermittelt die Linienfarbe für die aktuelle Fortschrittslinie.

**Returns:**
java.awt.Color - die Linienfarbe für die aktuelle Fortschrittslinie.
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


Ermittelt das Linienmuster der aktuellen Fortschrittslinie. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Returns:**
int - das Linienmuster der aktuellen Fortschrittslinie.
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


Ermittelt die Farbe der anderen Fortschrittslinie.

**Returns:**
java.awt.Color - die Farbe der anderen Fortschrittslinie.
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


Ermittelt das Linienmuster für die andere Fortschrittslinie.

**Returns:**
int - das Linienmuster für die andere Fortschrittslinie.
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


Ermittelt die Farbe des anderen Fortschrittspunkts.

**Returns:**
java.awt.Color - die Farbe des anderen Fortschrittspunkts.
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


Ermittelt die Form des Fortschrittspunkts der anderen Fortschrittslinie.

**Returns:**
int - die Form des Fortschrittspunkts der anderen Fortschrittslinie.
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


Ermittelt die Farbe des Fortschrittspunkts.

**Returns:**
java.awt.Color - die Farbe des Fortschrittspunkts.
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


Ermittelt die Form des Fortschrittspunkts. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Returns:**
int - die Form des Fortschrittspunkts.
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


Ermittelt das wiederkehrende Intervall. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


Ermittelt die Liste der ausgewählten Daten, für die Fortschrittslinien angezeigt werden sollen.

**Returns:**
java.util.List&lt;java.util.Date&gt; - die Liste der ausgewählten Daten, für die Fortschrittslinien angezeigt werden sollen.
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


Ermittelt einen Wert, der angibt, ob das Datum für jede Fortschrittslinie angezeigt werden soll.

**Returns:**
boolean - ein Wert, der angibt, ob das Datum für jede Fortschrittslinie angezeigt wird.
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


Ermittelt einen Wert, der angibt, ob Fortschrittslinien für den Basisplan oder den Ist-Stand angezeigt werden sollen.

**Returns:**
boolean - ein Wert, der angibt, ob Fortschrittslinien für den Basisplan oder den Ist-Zustand angezeigt werden.
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


Legt einen Wert fest, der angibt, ob Fortschrittslinien für den Basisplan oder den Ist-Stand angezeigt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Fortschrittslinien für den Basisplan oder den Ist-Zustand angezeigt werden. |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


Legt das Datum fest, ab dem Fortschrittslinien angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das Datum, ab dem Fortschrittslinien angezeigt werden sollen. |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


Legt einen Wert fest, der angibt, ob Fortschrittslinien ab dem Beginn des Projektstartdatums angezeigt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Fortschrittslinien ab dem Beginn des Projektstartdatums angezeigt werden sollen. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Legt das Datumsformat fest ([DateLabel](../../com.aspose.tasks/datelabel)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | int | das Datumsformat ([DateLabel](../../com.aspose.tasks/datelabel)). |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


Legt einen Wert fest, der angibt, ob die Fortschrittslinie am aktuellen Datum angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Fortschrittslinie am aktuellen Datum angezeigt wird. |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


Legt einen Wert fest, der angibt, ob die Fortschrittslinie in wiederkehrenden Intervallen angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob die Fortschrittslinie in wiederkehrenden Intervallen angezeigt werden soll. |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


Legt einen Wert fest, der angibt, ob die Fortschrittslinien an den ausgewählten Daten angezeigt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob die Fortschrittslinien an den ausgewählten Daten angezeigt werden sollen. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Legt die für das Fortschrittslinien-Label verwendete Schriftart fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Die für das Fortschrittslinien-Label verwendete Schriftart. |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


Legt die Linienfarbe für die aktuelle Fortschrittslinie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color | Die Linienfarbe für die aktuelle Fortschrittslinie. |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


Legt das Linienmuster der aktuellen Fortschrittslinie fest. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Das Linienmuster der aktuellen Fortschrittslinie. |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


Legt die Farbe der anderen Fortschrittslinie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color | Die Farbe der anderen Fortschrittslinie. |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


Legt das Linienmuster für die andere Fortschrittslinie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Das Linienmuster für die andere Fortschrittslinie. |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


Legt die Farbe des anderen Fortschrittspunkts fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color | Die Farbe des anderen Fortschrittspunkts. |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


Legt die Form des Fortschrittspunkts der anderen Fortschrittslinie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Die Form des Fortschrittspunkts der anderen Fortschrittslinie. |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


Legt die Farbe des Fortschrittspunkts fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color | Die Farbe des Fortschrittspunkts. |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


Legt die Form des Fortschrittspunkts fest. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Die Form des Fortschrittspunkts. |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


Legt das wiederkehrende Intervall fest. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | Das wiederkehrende Intervall. |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


Legt einen Wert fest, der angibt, ob das Datum für jede Fortschrittslinie angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob das Datum für jede Fortschrittslinie angezeigt werden soll. |

