---
title: "ProgressLines"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa líneas de progreso en una vista de diagrama de Gantt."
type: docs
weight: 219
url: /es/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

Representa líneas de progreso en una vista de diagrama de Gantt.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | Obtiene la fecha desde la cual mostrar las líneas de progreso. |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | Obtiene un valor que indica si se deben mostrar líneas de progreso desde el inicio de la fecha de inicio del proyecto. |
| [getDateFormat()](#getDateFormat--) | Obtiene el formato de fecha ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | Obtiene un valor que indica si se debe mostrar la línea de progreso en la fecha actual. |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | Obtiene un valor que indica si se debe mostrar la línea de progreso en intervalos recurrentes. |
| [getDisplaySelected()](#getDisplaySelected--) | Obtiene un valor que indica si se deben mostrar líneas de progreso en las fechas seleccionadas. |
| [getFont()](#getFont--) | Obtiene la fuente utilizada para la etiqueta de la línea de progreso. |
| [getLineColor()](#getLineColor--) | Obtiene el color de línea para la línea de progreso actual. |
| [getLinePattern()](#getLinePattern--) | Obtiene el patrón de línea de la línea de progreso actual. |
| [getOtherLineColor()](#getOtherLineColor--) | Obtiene el color de otra línea de progreso. |
| [getOtherLinePattern()](#getOtherLinePattern--) | Obtiene el patrón de línea para otra línea de progreso. |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | Obtiene el color de otro punto de progreso. |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | Obtiene la forma del punto de progreso de otra línea de progreso. |
| [getProgressPointColor()](#getProgressPointColor--) | Obtiene el color del punto de progreso. |
| [getProgressPointShape()](#getProgressPointShape--) | Obtiene la forma del punto de progreso. |
| [getRecurringInterval()](#getRecurringInterval--) | Obtiene el intervalo recurrente. |
| [getSelectedDates()](#getSelectedDates--) | Obtiene la lista de fechas seleccionadas para las que se mostrarán líneas de progreso. |
| [getShowDate()](#getShowDate--) | Obtiene un valor que indica si se debe mostrar la fecha para cada línea de progreso. |
| [isBaselinePlan()](#isBaselinePlan--) | Obtiene un valor que indica si se deben mostrar líneas de progreso para el plan base o real. |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | Establece un valor que indica si se deben mostrar líneas de progreso para el plan base o real. |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | Establece la fecha a partir de la cual se mostrarán líneas de progreso. |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | Establece un valor que indica si se deben mostrar líneas de progreso desde el inicio de la fecha de inicio del proyecto. |
| [setDateFormat(int value)](#setDateFormat-int-) | Establece el formato de fecha ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | Establece un valor que indica si se debe mostrar la línea de progreso en la fecha actual. |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | Establece un valor que indica si se debe mostrar la línea de progreso en intervalos recurrentes. |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | Establece un valor que indica si se deben mostrar líneas de progreso en las fechas seleccionadas. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Establece la fuente utilizada para la etiqueta de la línea de progreso. |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | Establece el color de la línea para la línea de progreso actual. |
| [setLinePattern(int value)](#setLinePattern-int-) | Establece el patrón de línea de la línea de progreso actual. |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | Establece el color de otra línea de progreso. |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | Establece el patrón de línea para otra línea de progreso. |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | Establece el color de otro punto de progreso. |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | Establece la forma del punto de progreso de otra línea de progreso. |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | Establece el color del punto de progreso. |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | Establece la forma del punto de progreso. |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | Establece el intervalo recurrente. |
| [setShowDate(boolean value)](#setShowDate-boolean-) | Establece un valor que indica si se muestra la fecha para cada línea de progreso. |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


Obtiene la fecha desde la cual mostrar las líneas de progreso.

**Returns:**
java.util.Date - la fecha a partir de la cual se muestran las líneas de progreso.
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


Obtiene un valor que indica si se deben mostrar líneas de progreso desde el inicio de la fecha de inicio del proyecto.

**Returns:**
boolean - un valor que indica si se muestran las líneas de progreso desde el inicio de la fecha de comienzo del proyecto.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Obtiene el formato de fecha ([DateLabel](../../com.aspose.tasks/datelabel)).

**Returns:**
int - el formato de fecha ([DateLabel](../../com.aspose.tasks/datelabel)).
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


Obtiene un valor que indica si se debe mostrar la línea de progreso en la fecha actual.

**Returns:**
boolean - un valor que indica si se muestra la línea de progreso en la fecha actual.
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


Obtiene un valor que indica si se debe mostrar la línea de progreso en intervalos recurrentes.

**Returns:**
boolean - un valor que indica si se muestra la línea de progreso en intervalos recurrentes.
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


Obtiene un valor que indica si se deben mostrar líneas de progreso en las fechas seleccionadas.

**Returns:**
boolean - un valor que indica si se muestran las líneas de progreso en las fechas seleccionadas.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Obtiene la fuente utilizada para la etiqueta de la línea de progreso.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


Obtiene el color de línea para la línea de progreso actual.

**Returns:**
java.awt.Color - el color de la línea para la línea de progreso actual.
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


Obtiene el patrón de línea de la línea de progreso actual. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Returns:**
int - el patrón de línea de la línea de progreso actual.
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


Obtiene el color de otra línea de progreso.

**Returns:**
java.awt.Color - el color de otra línea de progreso.
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


Obtiene el patrón de línea para otra línea de progreso.

**Returns:**
int - el patrón de línea para otra línea de progreso.
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


Obtiene el color de otro punto de progreso.

**Returns:**
java.awt.Color - el color de otro punto de progreso.
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


Obtiene la forma del punto de progreso de otra línea de progreso.

**Returns:**
int - la forma del punto de progreso de otra línea de progreso.
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


Obtiene el color del punto de progreso.

**Returns:**
java.awt.Color - el color del punto de progreso.
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


Obtiene la forma del punto de progreso. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Returns:**
int - la forma del punto de progreso.
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


Obtiene el intervalo recurrente. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


Obtiene la lista de fechas seleccionadas para las que se mostrarán líneas de progreso.

**Returns:**
java.util.List&lt;java.util.Date&gt; - la lista de fechas seleccionadas para mostrar líneas de progreso.
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


Obtiene un valor que indica si se debe mostrar la fecha para cada línea de progreso.

**Returns:**
boolean - un valor que indica si se muestra la fecha para cada línea de progreso.
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


Obtiene un valor que indica si se deben mostrar líneas de progreso para el plan base o real.

**Returns:**
boolean - un valor que indica si se muestran líneas de progreso para el plan base o real.
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


Establece un valor que indica si se deben mostrar líneas de progreso para el plan base o real.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se muestran líneas de progreso para el plan base o real. |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


Establece la fecha a partir de la cual se mostrarán líneas de progreso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | la fecha a partir de la cual se muestran las líneas de progreso. |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


Establece un valor que indica si se deben mostrar líneas de progreso desde el inicio de la fecha de inicio del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se muestran líneas de progreso desde el inicio de la fecha de inicio del proyecto. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Establece el formato de fecha ([DateLabel](../../com.aspose.tasks/datelabel)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | int | el formato de fecha ([DateLabel](../../com.aspose.tasks/datelabel)). |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


Establece un valor que indica si se debe mostrar la línea de progreso en la fecha actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se muestra la línea de progreso en la fecha actual. |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


Establece un valor que indica si se debe mostrar la línea de progreso en intervalos recurrentes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se muestra la línea de progreso en intervalos recurrentes. |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


Establece un valor que indica si se deben mostrar líneas de progreso en las fechas seleccionadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se muestran líneas de progreso en las fechas seleccionadas. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Establece la fuente utilizada para la etiqueta de la línea de progreso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | la fuente utilizada para la etiqueta de la línea de progreso. |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


Establece el color de la línea para la línea de progreso actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color | el color de línea para la línea de progreso actual. |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


Establece el patrón de línea de la línea de progreso actual. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el patrón de línea de la línea de progreso actual. |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


Establece el color de otra línea de progreso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color | el color de la otra línea de progreso. |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


Establece el patrón de línea para otra línea de progreso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el patrón de línea para la otra línea de progreso. |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


Establece el color de otro punto de progreso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color | el color del otro punto de progreso. |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


Establece la forma del punto de progreso de otra línea de progreso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la forma del punto de progreso de la otra línea de progreso. |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


Establece el color del punto de progreso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color | el color del punto de progreso. |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


Establece la forma del punto de progreso. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la forma del punto de progreso. |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


Establece el intervalo recurrente. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | el intervalo recurrente. |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


Establece un valor que indica si se muestra la fecha para cada línea de progreso.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se muestra la fecha para cada línea de progreso. |

