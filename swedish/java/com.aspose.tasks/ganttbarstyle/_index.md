---
title: "GanttBarStyle"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en stapelstil som används av MSP i Gantt-diagramvyn."
type: docs
weight: 109
url: /sv/java/com.aspose.tasks/ganttbarstyle/
---

**Inheritance:**
java.lang.Object
```
public class GanttBarStyle
```

Representerar en stapelstil som används av MSP i Gantt-diagramvyn.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [GanttBarStyle()](#GanttBarStyle--) | Initierar en ny instans av klassen [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getBottomBarTextConverter()](#getBottomBarTextConverter--) | Hämtar en användardefinierad konverterare för att få text som ska renderas längst ner på uppgiftens stapel. |
| [getBottomField()](#getBottomField--) | Hämtar data som ska visas längst ner på stapeln. |
| [getEndShape()](#getEndShape--) | Hämtar en slutform för stapeln. |
| [getEndShapeColor()](#getEndShapeColor--) | Hämtar en färg på slutformen. |
| [getEndShapeType()](#getEndShapeType--) | Hämtar en typ av slutformen. |
| [getFrom()](#getFrom--) | Hämtar en startpunktsposition för gantt-fältet. |
| [getInsideBarTextConverter()](#getInsideBarTextConverter--) | Hämtar en användardefinierad konverterare för att få text att renderas inuti uppgiftens stapel. |
| [getInsideField()](#getInsideField--) | Hämtar data som ska visas inuti stapeln. |
| [getLeftBarTextConverter()](#getLeftBarTextConverter--) | Hämtar en användardefinierad konverterare för att få text att renderas till vänster om uppgiftens stapel. |
| [getLeftField()](#getLeftField--) | Hämtar data som ska visas till vänster om stapeln. |
| [getMiddleFillPattern()](#getMiddleFillPattern--) | Hämtar ett fyllningsmönster för gantt-fältet. |
| [getMiddleShape()](#getMiddleShape--) | Hämtar en mittform för stapeln. |
| [getMiddleShapeColor()](#getMiddleShapeColor--) | Hämtar en färg för mittformen. |
| [getName()](#getName--) | Hämtar ett namn på stilen. |
| [getParentStyle()](#getParentStyle--) | Hämtar föräldra‑ (eller gemensam) stil för anpassad uppgiftsspecifik stil. |
| [getRightBarTextConverter()](#getRightBarTextConverter--) | Hämtar en användardefinierad konverterare för att få text att renderas till höger om uppgiftens stapel. |
| [getRightField()](#getRightField--) | Hämtar data som ska visas till höger om stapeln. |
| [getRow()](#getRow--) | Hämtar ett radnummer. |
| [getShowForCategories()](#getShowForCategories--) | Hämtar uppgiftskategorier som stilen tillämpas på. |
| [getShowForTaskUid()](#getShowForTaskUid--) | Hämtar unikt ID för en uppgift som stilen tillämpas på. |
| [getStartShape()](#getStartShape--) | Hämtar en startform för stapeln. |
| [getStartShapeColor()](#getStartShapeColor--) | Hämtar en färg för startformen. |
| [getStartShapeType()](#getStartShapeType--) | Hämtar en typ av startformen. |
| [getTo()](#getTo--) | Hämtar en slutpunktsposition för gantt-fältet. |
| [getTopBarTextConverter()](#getTopBarTextConverter--) | Hämtar en användardefinierad konverterare för att få text att renderas ovanpå uppgiftens stapel. |
| [getTopField()](#getTopField--) | Hämtar data som ska visas ovanpå stapeln. |
| [setBottomBarTextConverter(TaskBarTextConverter value)](#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Ställer in en användardefinierad konverterare för att få text att renderas längst ner på uppgiftens stapel. |
| [setBottomField(int value)](#setBottomField-int-) | Ställer in data som ska visas längst ner på stapeln. |
| [setEndShape(int value)](#setEndShape-int-) | Ställer in en slutform för stapeln. |
| [setEndShapeColor(Color value)](#setEndShapeColor-java.awt.Color-) | Anger en färg på slutformen. |
| [setEndShapeType(int value)](#setEndShapeType-int-) | Anger en typ av slutformen. |
| [setFrom(int value)](#setFrom-int-) | Anger startpunktens position för gantt-stapeln. |
| [setInsideBarTextConverter(TaskBarTextConverter value)](#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Anger en användardefinierad konverterare för att hämta text som ska renderas inuti uppgiftens stapel. |
| [setInsideField(int value)](#setInsideField-int-) | Anger data som ska visas inuti stapeln. |
| [setLeftBarTextConverter(TaskBarTextConverter value)](#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Anger en användardefinierad konverterare för att hämta text som ska renderas till vänster om uppgiftens stapel. |
| [setLeftField(int value)](#setLeftField-int-) | Anger data som ska visas till vänster om stapeln. |
| [setMiddleFillPattern(int value)](#setMiddleFillPattern-int-) | Anger ett fyllningsmönster för gantt-stapeln. |
| [setMiddleShape(int value)](#setMiddleShape-int-) | Anger en mittform för stapeln. |
| [setMiddleShapeColor(Color value)](#setMiddleShapeColor-java.awt.Color-) | Anger en färg på mittformen. |
| [setName(String value)](#setName-java.lang.String-) | Anger ett namn på stilen. |
| [setParentStyle(GanttBarStyle value)](#setParentStyle-com.aspose.tasks.GanttBarStyle-) | Anger föräldra- (eller gemensam) stil för anpassad uppgiftsspecifik stil. |
| [setRightBarTextConverter(TaskBarTextConverter value)](#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Anger en användardefinierad konverterare för att hämta text som ska renderas till höger om uppgiftens stapel. |
| [setRightField(int value)](#setRightField-int-) | Anger data som ska visas till höger om stapeln. |
| [setRow(int value)](#setRow-int-) | Anger ett radnummer. |
| [setShowForCategories(List&lt;Integer&gt; value)](#setShowForCategories-java.util.List-java.lang.Integer--) | Anger uppgiftskategorier som stilen tillämpas på. |
| [setShowForTaskUid(Integer value)](#setShowForTaskUid-java.lang.Integer-) | Anger unikt ID för en uppgift som stilen tillämpas på. |
| [setStartShape(int value)](#setStartShape-int-) | Anger en startform för stapeln. |
| [setStartShapeColor(Color value)](#setStartShapeColor-java.awt.Color-) | Anger en färg på startformen. |
| [setStartShapeType(int value)](#setStartShapeType-int-) | Anger en typ av startformen. |
| [setTo(int value)](#setTo-int-) | Anger slutpunktens position för gantt-stapeln. |
| [setTopBarTextConverter(TaskBarTextConverter value)](#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Anger en användardefinierad konverterare för att hämta text som ska renderas ovanför uppgiftens stapel. |
| [setTopField(int value)](#setTopField-int-) | Anger data som ska visas ovanför stapeln. |
### GanttBarStyle() {#GanttBarStyle--}
```
public GanttBarStyle()
```


Initierar en ny instans av klassen [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

### getBottomBarTextConverter() {#getBottomBarTextConverter--}
```
public final TaskBarTextConverter getBottomBarTextConverter()
```


Hämtar en användardefinierad konverterare för att hämta text som ska renderas längst ner på uppgiftens stapel. Åsidosätter värdet för `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-))‑egenskapen.

--------------------

Sparas inte i MPP-format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the bottom of the task's bar.
### getBottomField() {#getBottomField--}
```
public final int getBottomField()
```


Hämtar data som ska visas längst ner på stapeln. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data som ska visas längst ner på stapeln.
### getEndShape() {#getEndShape--}
```
public final int getEndShape()
```


Hämtar en slutform för stapeln.

**Returns:**
int - en slutform på stapeln.
### getEndShapeColor() {#getEndShapeColor--}
```
public final Color getEndShapeColor()
```


Hämtar en färg på slutformen.

**Returns:**
java.awt.Color - en färg på slutformen.
### getEndShapeType() {#getEndShapeType--}
```
public final int getEndShapeType()
```


Hämtar en typ av slutformen. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Returns:**
int - en typ av slutformen.
### getFrom() {#getFrom--}
```
public final int getFrom()
```


Hämtar startpunktens position för Gantt-stapeln. [Field](../../com.aspose.tasks/field).

**Returns:**
int - en startpunktposition för Gantt-stapeln.
### getInsideBarTextConverter() {#getInsideBarTextConverter--}
```
public final TaskBarTextConverter getInsideBarTextConverter()
```


Hämtar användardefinierad konverterare för att få text att renderas inuti uppgiftens stapel. Åsidosätter värdet för egenskapen `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)).

--------------------

Sparas inte i MPP-format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render inside of the task's bar.
### getInsideField() {#getInsideField--}
```
public final int getInsideField()
```


Hämtar data som ska visas inuti stapeln. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data som ska visas inuti stapeln.
### getLeftBarTextConverter() {#getLeftBarTextConverter--}
```
public final TaskBarTextConverter getLeftBarTextConverter()
```


Hämtar användardefinierad konverterare för att få text att renderas till vänster om uppgiftens stapel. Åsidosätter värdet för egenskapen `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)).

--------------------

Sparas inte i MPP-format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the left of the task's bar.
### getLeftField() {#getLeftField--}
```
public final int getLeftField()
```


Hämtar data som ska visas till vänster om stapeln. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data som ska visas till vänster om stapeln.
### getMiddleFillPattern() {#getMiddleFillPattern--}
```
public final int getMiddleFillPattern()
```


Hämtar ett fyllningsmönster för gantt-fältet.

**Returns:**
int - ett fyllningsmönster för Gantt-stapeln.
### getMiddleShape() {#getMiddleShape--}
```
public final int getMiddleShape()
```


Hämtar en mittform för stapeln.

**Returns:**
int - en mittform på stapeln.
### getMiddleShapeColor() {#getMiddleShapeColor--}
```
public final Color getMiddleShapeColor()
```


Hämtar en färg för mittformen.

**Returns:**
java.awt.Color - en färg på mittformen.
### getName() {#getName--}
```
public final String getName()
```


Hämtar ett namn på stilen.

**Returns:**
java.lang.String - ett namn på stilen.
### getParentStyle() {#getParentStyle--}
```
public final GanttBarStyle getParentStyle()
```


Hämtar föräldra‑ (eller gemensam) stil för anpassad uppgiftsspecifik stil.

--------------------

En uppgift kan ha flera anpassade stilar med olika föräldrastilar. Till exempel, föreställ dig en uppgift med en anpassad stil som har föräldrastilen "Critical" och en annan stil med föräldrastilen "Normal". Enkelt uttryckt, om uppgiften är kritisk tillämpas den första stilen. Om uppgiften blir icke‑kritisk tillämpas den andra stilen (denna logik är ärvd från Microsoft Project Professional).

**Returns:**
[GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) - parent (or common) style for custom task-specific style.
### getRightBarTextConverter() {#getRightBarTextConverter--}
```
public final TaskBarTextConverter getRightBarTextConverter()
```


Hämtar användardefinierad konverterare för att få text att renderas till höger om uppgiftens stapel. Åsidosätter värdet för egenskapen `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)).

--------------------

Sparas inte i MPP-format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the right of the task's bar.
### getRightField() {#getRightField--}
```
public final int getRightField()
```


Hämtar data som ska visas till höger om stapeln. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data som ska visas till höger om stapeln.
### getRow() {#getRow--}
```
public final int getRow()
```


Hämtar ett radnummer.

--------------------

Kan vara från 1 till 4 (1 är standardvärde).

**Returns:**
int - ett radnummer.
### getShowForCategories() {#getShowForCategories--}
```
public final List<Integer> getShowForCategories()
```


Hämtar uppgiftskategorier som stilen tillämpas på. Gäller för föräldra‑ (eller gemensamma) stilar för staplar i Gantt‑diagrammet (se `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - uppgiftskategorier som stilen tillämpas på.
### getShowForTaskUid() {#getShowForTaskUid--}
```
public final Integer getShowForTaskUid()
```


Hämtar unikt ID för en uppgift som stilen tillämpas på. Är tillämplig för uppgiftsspecifika stilar för staplar i Gantt-diagram (se `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose/tasks/ganttchartview\#getCustomBarStyles--))).

**Returns:**
java.lang.Integer - Unikt ID för en uppgift som stilen tillämpas på.
### getStartShape() {#getStartShape--}
```
public final int getStartShape()
```


Hämtar en startform för stapeln.

**Returns:**
int - en startform för stapeln.
### getStartShapeColor() {#getStartShapeColor--}
```
public final Color getStartShapeColor()
```


Hämtar en färg för startformen.

**Returns:**
java.awt.Color - en färg på startformen.
### getStartShapeType() {#getStartShapeType--}
```
public final int getStartShapeType()
```


Hämtar en typ av startformen.

**Returns:**
int - en typ av startformen.
### getTo() {#getTo--}
```
public final int getTo()
```


Hämtar en slutpunktsposition för gantt-fältet.

**Returns:**
int - en slutpunktsposition för Gantt-stapeln.
### getTopBarTextConverter() {#getTopBarTextConverter--}
```
public final TaskBarTextConverter getTopBarTextConverter()
```


Hämtar användardefinierad konverterare för att få text att renderas högst upp på uppgiftens stapel. Åsidosätter värdet av egenskapen `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)).

--------------------

Sparas inte i MPP-format.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the top of the task's bar.
### getTopField() {#getTopField--}
```
public final int getTopField()
```


Hämtar data som ska visas ovanpå stapeln.

**Returns:**
int - data som ska visas högst upp på stapeln.
### setBottomBarTextConverter(TaskBarTextConverter value) {#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setBottomBarTextConverter(TaskBarTextConverter value)
```


Ställer in användardefinierad konverterare för att få text att renderas längst ner på uppgiftens stapel. Åsidosätter värdet av egenskapen `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)).

--------------------

Sparas inte i MPP-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | användardefinierad konverterare för att få text att renderas längst ner på uppgiftens stapel. |

### setBottomField(int value) {#setBottomField-int-}
```
public final void setBottomField(int value)
```


Ställer in data som ska visas längst ner på stapeln. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | data som ska visas längst ner på stapeln. |

### setEndShape(int value) {#setEndShape-int-}
```
public final void setEndShape(int value)
```


Ställer in en slutform för stapeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en slutform för stapeln. |

### setEndShapeColor(Color value) {#setEndShapeColor-java.awt.Color-}
```
public final void setEndShapeColor(Color value)
```


Anger en färg på slutformen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color | en färg på slutformen. |

### setEndShapeType(int value) {#setEndShapeType-int-}
```
public final void setEndShapeType(int value)
```


Ställer in en typ av slutformen. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en typ av slutformen. |

### setFrom(int value) {#setFrom-int-}
```
public final void setFrom(int value)
```


Ställer in en startpunktsposition för Gantt-stapeln. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en startpunktsposition för Gantt-stapeln. |

### setInsideBarTextConverter(TaskBarTextConverter value) {#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setInsideBarTextConverter(TaskBarTextConverter value)
```


Ställer in användardefinierad konverterare för att få text att renderas inuti uppgiftens stapel. Åsidosätter värdet av egenskapen `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)).

--------------------

Sparas inte i MPP-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | användardefinierad konverterare för att få text att renderas inuti uppgiftens stapel. |

### setInsideField(int value) {#setInsideField-int-}
```
public final void setInsideField(int value)
```


Ställer in data som ska visas inuti stapeln. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | data som ska visas inuti stapeln. |

### setLeftBarTextConverter(TaskBarTextConverter value) {#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setLeftBarTextConverter(TaskBarTextConverter value)
```


Ställer in användardefinierad konverterare för att få text att renderas till vänster om uppgiftens stapel. Åsidosätter värdet av egenskapen `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)).

--------------------

Sparas inte i MPP-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | användardefinierad konverterare för att få text att renderas till vänster om uppgiftens stapel. |

### setLeftField(int value) {#setLeftField-int-}
```
public final void setLeftField(int value)
```


Ställer in data som ska visas till vänster om stapeln. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | data som ska visas till vänster om stapeln. |

### setMiddleFillPattern(int value) {#setMiddleFillPattern-int-}
```
public final void setMiddleFillPattern(int value)
```


Anger ett fyllningsmönster för gantt-stapeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett fyllningsmönster för gantt‑stapeln. |

### setMiddleShape(int value) {#setMiddleShape-int-}
```
public final void setMiddleShape(int value)
```


Anger en mittform för stapeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en mittform av stapeln. |

### setMiddleShapeColor(Color value) {#setMiddleShapeColor-java.awt.Color-}
```
public final void setMiddleShapeColor(Color value)
```


Anger en färg på mittformen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color | en färg på mittformen. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Anger ett namn på stilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett namn på stilen. |

### setParentStyle(GanttBarStyle value) {#setParentStyle-com.aspose.tasks.GanttBarStyle-}
```
public final void setParentStyle(GanttBarStyle value)
```


Anger föräldra- (eller gemensam) stil för anpassad uppgiftsspecifik stil.

--------------------

En uppgift kan ha flera anpassade stilar med olika föräldrastilar. Till exempel, föreställ dig en uppgift med en anpassad stil som har föräldrastilen "Critical" och en annan stil med föräldrastilen "Normal". Enkelt uttryckt, om uppgiften är kritisk tillämpas den första stilen. Om uppgiften blir icke‑kritisk tillämpas den andra stilen (denna logik är ärvd från Microsoft Project Professional).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) | föräldra‑ (eller gemensam) stil för anpassad uppgiftsspecifik stil. |

### setRightBarTextConverter(TaskBarTextConverter value) {#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setRightBarTextConverter(TaskBarTextConverter value)
```


Ställer in användardefinierad konverterare för att hämta text som ska renderas till höger om uppgiftens stapel. Åsidosätter värdet för `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) egenskapen.

--------------------

Sparas inte i MPP-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | användardefinierad konverterare för att hämta text som ska renderas till höger om uppgiftens stapel. |

### setRightField(int value) {#setRightField-int-}
```
public final void setRightField(int value)
```


Ställer in data som ska visas till höger om stapeln. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | data som ska visas till höger om stapeln. |

### setRow(int value) {#setRow-int-}
```
public final void setRow(int value)
```


Anger ett radnummer.

--------------------

Kan vara från 1 till 4 (1 är standardvärde).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett radnummer. |

### setShowForCategories(List&lt;Integer&gt; value) {#setShowForCategories-java.util.List-java.lang.Integer--}
```
public final void setShowForCategories(List<Integer> value)
```


Ställer in uppgiftskategorier som stilen ska tillämpas på. Gäller för föräldra‑ (eller gemensamma) stilar för staplar i Gantt‑diagram (se `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.List&lt;java.lang.Integer&gt; | uppgiftskategorier som stilen tillämpas på. |

### setShowForTaskUid(Integer value) {#setShowForTaskUid-java.lang.Integer-}
```
public final void setShowForTaskUid(Integer value)
```


Ställer in unikt ID för en uppgift som stilen ska tillämpas på. Gäller för uppgiftsspecifika stapelstilar i Gantt‑diagram (se `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Integer | Unikt ID för en uppgift som stilen tillämpas på. |

### setStartShape(int value) {#setStartShape-int-}
```
public final void setStartShape(int value)
```


Anger en startform för stapeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en startform för stapeln. |

### setStartShapeColor(Color value) {#setStartShapeColor-java.awt.Color-}
```
public final void setStartShapeColor(Color value)
```


Anger en färg på startformen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color | en färg på startformen. |

### setStartShapeType(int value) {#setStartShapeType-int-}
```
public final void setStartShapeType(int value)
```


Anger en typ av startformen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en typ av startformen. |

### setTo(int value) {#setTo-int-}
```
public final void setTo(int value)
```


Anger slutpunktens position för gantt-stapeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en slutpunktsposition för gantt‑stapeln. |

### setTopBarTextConverter(TaskBarTextConverter value) {#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setTopBarTextConverter(TaskBarTextConverter value)
```


Ställer in användardefinierad konverterare för att hämta text som ska renderas högst upp på uppgiftens stapel. Åsidosätter värdet för `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)) egenskapen.

--------------------

Sparas inte i MPP-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | användardefinierad konverterare för att hämta text som ska renderas högst upp på uppgiftens stapel. |

### setTopField(int value) {#setTopField-int-}
```
public final void setTopField(int value)
```


Anger data som ska visas ovanför stapeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | data som ska visas högst upp på stapeln. |

