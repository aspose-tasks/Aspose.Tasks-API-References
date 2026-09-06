---
title: "TimephasedData"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa datos faseados en el tiempo."
type: docs
weight: 320
url: /es/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Representa datos faseados en el tiempo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose/tasks/timephaseddata). |
## Métodos

| Método | Descripción |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Crea e inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose.tasks/timephaseddata) para datos temporales basados en costos. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Crea e inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose.tasks/timephaseddata) para datos temporales basados en costos. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Crea e inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose.tasks/timephaseddata) para datos temporales basados en unidades de una asignación de un recurso material. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Crea e inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose.tasks/timephaseddata) para datos temporales basados en trabajo. |
| [getFinish()](#getFinish--) | Obtiene la fecha de finalización de un período de datos temporales. |
| [getStart()](#getStart--) | Obtiene la fecha de inicio de un período de datos temporales. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Obtiene el tipo de un dato temporal. |
| [getUid()](#getUid--) | Obtiene el identificador único de un dato temporal |
| [getUnit()](#getUnit--) | Obtiene la unidad de tiempo de un período de datos temporales. |
| [getValue()](#getValue--) | Obtiene el valor por unidad de tiempo de un período de datos temporales. |
| [getValueToCost()](#getValueToCost--) | Obtiene la instancia `double` que representa el valor de cadena de este objeto. |
| [getValueToDuration()](#getValueToDuration--) | Obtiene la instancia double que representa el valor de cadena de este objeto. |
| [getValueToUnits()](#getValueToUnits--) | Obtiene la instancia `double` que representa el valor de cadena de este objeto para datos temporales basados en unidades. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Establece la fecha de finalización de un período de datos temporales. |
| [setStart(Date value)](#setStart-java.util.Date-) | Establece la fecha de inicio de un período de datos temporales. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Establece el tipo de un dato temporal. |
| [setUid(int value)](#setUid-int-) | Establece el identificador único de un dato temporal |
| [setUnit(byte value)](#setUnit-byte-) | Establece la unidad de tiempo de un período de datos temporales. |
| [setValue(String value)](#setValue-java.lang.String-) | Establece el valor por unidad de tiempo de un período de datos temporales. |
| [setValueToCost(double value)](#setValueToCost-double-) | Instancia `double` que representa el valor de cadena de este objeto. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose/tasks/timephaseddata).

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Crea e inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose.tasks/timephaseddata) para datos temporales basados en costos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | int | UID de la tarea. |
| inicio | java.util.Date | fecha y hora de inicio. |
| finalizar | java.util.Date | Fecha y hora de finalización. |
| valor | double | Valor de costo. |
| type | byte | Tipo de datos temporales. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Crea e inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose.tasks/timephaseddata) para datos temporales basados en costos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | int | UID de la tarea. |
| inicio | java.util.Date | fecha y hora de inicio. |
| finalizar | java.util.Date | Fecha y hora de finalización. |
| valor | double | Valor de costo. |
| unidadDeTiempo | byte | Tipo de unidad de tiempo. |
| type | byte | Tipo de datos temporales. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Crea e inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose.tasks/timephaseddata) para datos temporales basados en unidades de una asignación de un recurso material.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | int | UID de la tarea. |
| inicio | java.util.Date | Fecha y hora de inicio. |
| finalizar | java.util.Date | Fecha y hora de finalización. |
| unidades | double | Número de unidades. |
| type | byte | Tipo de datos temporales. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Crea e inicializa una nueva instancia de la clase [TimephasedData](../../com.aspose.tasks/timephaseddata) para datos temporales basados en trabajo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | int | UID de la tarea. |
| inicio | java.util.Date | fecha y hora de inicio. |
| finalizar | java.util.Date | Fecha y hora de finalización. |
| valor | double | Valor del intervalo de tiempo. |
| unidadDeTiempo | byte | Tipo de unidad de tiempo. |
| type | byte | Tipo de datos temporales. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Obtiene la fecha de finalización de un período de datos temporales.

**Returns:**
java.util.Date - la fecha de finalización de un período de datos con fase de tiempo.
### getStart() {#getStart--}
```
public final Date getStart()
```


Obtiene la fecha de inicio de un período de datos temporales.

**Returns:**
java.util.Date - la fecha de inicio de un período de datos con fase de tiempo.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Obtiene el tipo de un dato temporal.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) la propiedad será borrada si no es adecuada para el tipo especificado aquí.

**Returns:**
byte - el tipo de un dato con fase de tiempo.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtiene el identificador único de un dato temporal

**Returns:**
int - el identificador único de un dato con fase de tiempo
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Obtiene la unidad de tiempo de un período de datos temporales.

**Returns:**
byte - la unidad de tiempo de un período de datos con fase de tiempo.
### getValue() {#getValue--}
```
public final String getValue()
```


Obtiene el valor por unidad de tiempo de un período de datos temporales.

**Returns:**
java.lang.String - el valor por unidad de tiempo para un período de datos con fase de tiempo.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


Obtiene la instancia `double` que representa el valor de cadena de este objeto.

**Returns:**
double - una representación de punto flotante del objeto.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


Obtiene la instancia double que representa el valor de cadena de este objeto.

**Returns:**
double - una representación de intervalo de tiempo del objeto.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Obtiene la instancia `double` que representa el valor de cadena de este objeto para datos temporales basados en unidades.

**Returns:**
double - una representación de punto flotante de este objeto.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Establece la fecha de finalización de un período de datos temporales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | la fecha de finalización de un período de datos con fase de tiempo. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Establece la fecha de inicio de un período de datos temporales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | la fecha de inicio de un período de datos con fase de tiempo. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Establece el tipo de un dato temporal.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) la propiedad será borrada si no es adecuada para el tipo especificado aquí.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte | el tipo de un dato con fase de tiempo. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Establece el identificador único de un dato temporal

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el identificador único de un dato con fase de tiempo |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Establece la unidad de tiempo de un período de datos temporales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte | la unidad de tiempo de un período de datos con fase de tiempo. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Establece el valor por unidad de tiempo de un período de datos temporales.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el valor por unidad de tiempo para un período de datos con fase de tiempo. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


Instancia `double` que representa el valor de cadena de este objeto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | Instancia `double` que representa el valor de cadena de este objeto. |

