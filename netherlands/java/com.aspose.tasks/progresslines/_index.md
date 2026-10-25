---
title: "ProgressLines"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Geeft voortgangslijnen weer in een Gantt-diagramweergave."
type: docs
weight: 219
url: /nl/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

Geeft voortgangslijnen weer in een Gantt-diagramweergave.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | Haalt de datum op vanaf wanneer voortgangslijnen worden weergegeven. |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | Haalt een waarde op die aangeeft of voortgangslijnen vanaf het begin van de projectstartdatum moeten worden weergegeven. |
| [getDateFormat()](#getDateFormat--) | Haalt het datumformaat op ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | Haalt een waarde op die aangeeft of de voortgangslijn op de huidige datum moet worden weergegeven. |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | Haalt een waarde op die aangeeft of de voortgangslijn op terugkerende intervallen moet worden weergegeven. |
| [getDisplaySelected()](#getDisplaySelected--) | Haalt een waarde op die aangeeft of voortgangslijnen op de geselecteerde data moeten worden weergegeven. |
| [getFont()](#getFont--) | Haalt het lettertype op dat wordt gebruikt voor het label van de voortgangslijn. |
| [getLineColor()](#getLineColor--) | Haalt de lijnekleur op voor de huidige voortgangslijn. |
| [getLinePattern()](#getLinePattern--) | Haalt het lijnpatroon op van de huidige voortgangslijn. |
| [getOtherLineColor()](#getOtherLineColor--) | Haalt de kleur op van een andere voortgangslijn. |
| [getOtherLinePattern()](#getOtherLinePattern--) | Haalt het lijnpatroon op voor een andere voortgangslijn. |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | Haalt de kleur op van een ander voortgangspunt. |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | Haalt de vorm van het voortgangspunt op van een andere voortgangslijn. |
| [getProgressPointColor()](#getProgressPointColor--) | Haalt de kleur op van het voortgangspunt. |
| [getProgressPointShape()](#getProgressPointShape--) | Haalt de vorm van het voortgangspunt op. |
| [getRecurringInterval()](#getRecurringInterval--) | Haalt het terugkerende interval op. |
| [getSelectedDates()](#getSelectedDates--) | Haalt de lijst met geselecteerde data op waarvoor voortgangslijnen moeten worden weergegeven. |
| [getShowDate()](#getShowDate--) | Haalt een waarde op die aangeeft of de datum voor elke voortgangslijn moet worden getoond. |
| [isBaselinePlan()](#isBaselinePlan--) | Haalt een waarde op die aangeeft of voortgangslijnen voor het basisplan of de werkelijke situatie moeten worden weergegeven. |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | Stelt een waarde in die aangeeft of voortgangslijnen voor het basisplan of de werkelijke situatie moeten worden weergegeven. |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | Stelt de datum in vanaf wanneer voortgangslijnen moeten worden weergegeven. |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | Stelt een waarde in die aangeeft of voortgangslijnen vanaf het begin van de projectstartdatum moeten worden weergegeven. |
| [setDateFormat(int value)](#setDateFormat-int-) | Stelt het datumformaat in ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | Stelt een waarde in die aangeeft of de voortgangslijn op de huidige datum moet worden weergegeven. |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | Stelt een waarde in die aangeeft of de voortgangslijn op terugkerende intervallen moet worden weergegeven. |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | Stelt een waarde in die aangeeft of voortgangslijnen op de geselecteerde data moeten worden weergegeven. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Stelt het lettertype in dat wordt gebruikt voor het label van de voortgangslijn. |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | Stelt de lijnekleur in voor de huidige voortgangslijn. |
| [setLinePattern(int value)](#setLinePattern-int-) | Stelt het lijnpatroon in van de huidige voortgangslijn. |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | Stelt de kleur in van de andere voortgangslijn. |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | Stelt het lijnpatroon in voor de andere voortgangslijn. |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | Stelt de kleur in van het andere voortgangspunt. |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | Stelt de vorm van het voortgangspunt in van de andere voortgangslijn. |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | Stelt de kleur in van het voortgangspunt. |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | Stelt de vorm van het voortgangspunt in. |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | Stelt het terugkerende interval in. |
| [setShowDate(boolean value)](#setShowDate-boolean-) | Stelt een waarde in die aangeeft of de datum voor elke voortgangslijn moet worden weergegeven. |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


Haalt de datum op vanaf wanneer voortgangslijnen worden weergegeven.

**Returns:**
java.util.Date - de datum vanaf wanneer voortgangslijnen moeten worden weergegeven.
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


Haalt een waarde op die aangeeft of voortgangslijnen vanaf het begin van de projectstartdatum moeten worden weergegeven.

**Returns:**
boolean - een waarde die aangeeft of voortgangslijnen moeten worden weergegeven vanaf het begin van de projectstartdatum.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Haalt het datumformaat op ([DateLabel](../../com.aspose.tasks/datelabel)).

**Returns:**
int - het datumformaat ([DateLabel](../../com.aspose.tasks/datelabel)).
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


Haalt een waarde op die aangeeft of de voortgangslijn op de huidige datum moet worden weergegeven.

**Returns:**
boolean - een waarde die aangeeft of de voortgangslijn moet worden weergegeven op de huidige datum.
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


Haalt een waarde op die aangeeft of de voortgangslijn op terugkerende intervallen moet worden weergegeven.

**Returns:**
boolean - een waarde die aangeeft of de voortgangslijn moet worden weergegeven op terugkerende intervallen.
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


Haalt een waarde op die aangeeft of voortgangslijnen op de geselecteerde data moeten worden weergegeven.

**Returns:**
boolean - een waarde die aangeeft of voortgangslijnen moeten worden weergegeven op de geselecteerde data.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Haalt het lettertype op dat wordt gebruikt voor het label van de voortgangslijn.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


Haalt de lijnekleur op voor de huidige voortgangslijn.

**Returns:**
java.awt.Color - de lijnekleur voor de huidige voortgangslijn.
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


Haalt het lijnpatroon op van de huidige voortgangslijn. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Returns:**
int - het lijnpatroon van de huidige voortgangslijn.
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


Haalt de kleur op van een andere voortgangslijn.

**Returns:**
java.awt.Color - de kleur van de andere voortgangslijn.
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


Haalt het lijnpatroon op voor een andere voortgangslijn.

**Returns:**
int - het lijnpatroon voor de andere voortgangslijn.
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


Haalt de kleur op van een ander voortgangspunt.

**Returns:**
java.awt.Color - de kleur van het andere voortgangspunt.
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


Haalt de vorm van het voortgangspunt op van een andere voortgangslijn.

**Returns:**
int - de vorm van het voortgangspunt van de andere voortgangslijn.
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


Haalt de kleur op van het voortgangspunt.

**Returns:**
java.awt.Color - de kleur van het voortgangspunt.
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


Haalt de vorm van het voortgangspunt op. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Returns:**
int - de vorm van het voortgangspunt.
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


Haalt het terugkerende interval op. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


Haalt de lijst met geselecteerde data op waarvoor voortgangslijnen moeten worden weergegeven.

**Returns:**
java.util.List&lt;java.util.Date&gt; - de lijst met geselecteerde datums waarvoor voortgangslijnen worden weergegeven.
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


Haalt een waarde op die aangeeft of de datum voor elke voortgangslijn moet worden getoond.

**Returns:**
boolean - een waarde die aangeeft of de datum voor elke voortgangslijn moet worden weergegeven.
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


Haalt een waarde op die aangeeft of voortgangslijnen voor het basisplan of de werkelijke situatie moeten worden weergegeven.

**Returns:**
boolean - een waarde die aangeeft of voortgangslijnen voor het basismodel of de werkelijke situatie moeten worden weergegeven.
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


Stelt een waarde in die aangeeft of voortgangslijnen voor het basisplan of de werkelijke situatie moeten worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of voortgangslijnen voor het basismodel of de werkelijke situatie moeten worden weergegeven. |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


Stelt de datum in vanaf wanneer voortgangslijnen moeten worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de datum vanaf wanneer voortgangslijnen worden weergegeven. |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


Stelt een waarde in die aangeeft of voortgangslijnen vanaf het begin van de projectstartdatum moeten worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of voortgangslijnen vanaf de startdatum van het project moeten worden weergegeven. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Stelt het datumformaat in ([DateLabel](../../com.aspose.tasks/datelabel)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | int | het datumformaat ([DateLabel](../../com.aspose.tasks/datelabel)). |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


Stelt een waarde in die aangeeft of de voortgangslijn op de huidige datum moet worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een voortgangslijn op de huidige datum moet worden weergegeven. |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


Stelt een waarde in die aangeeft of de voortgangslijn op terugkerende intervallen moet worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een voortgangslijn op terugkerende intervallen moet worden weergegeven. |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


Stelt een waarde in die aangeeft of voortgangslijnen op de geselecteerde data moeten worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of voortgangslijnen op de geselecteerde datums moeten worden weergegeven. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Stelt het lettertype in dat wordt gebruikt voor het label van de voortgangslijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | het lettertype dat wordt gebruikt voor het label van de voortgangslijn. |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


Stelt de lijnekleur in voor de huidige voortgangslijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color | de lijnekleur voor de huidige voortgangslijn. |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


Stelt het lijnpatroon van de huidige voortgangslijn in. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het lijnpatroon van de huidige voortgangslijn. |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


Stelt de kleur in van de andere voortgangslijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color | de kleur van de andere voortgangslijn. |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


Stelt het lijnpatroon in voor de andere voortgangslijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het lijnpatroon voor de andere voortgangslijn. |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


Stelt de kleur in van het andere voortgangspunt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color | de kleur van het andere voortgangspunt. |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


Stelt de vorm van het voortgangspunt in van de andere voortgangslijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de vorm van het voortgangspunt van de andere voortgangslijn. |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


Stelt de kleur in van het voortgangspunt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color | de kleur van het voortgangspunt. |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


Stelt de vorm van het voortgangspunt in. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de vorm van het voortgangspunt. |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


Stelt het terugkerende interval in. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | het terugkerende interval. |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


Stelt een waarde in die aangeeft of de datum voor elke voortgangslijn moet worden weergegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de datum moet worden weergegeven voor elke voortgangslijn. |

