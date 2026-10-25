---
title: "TimephasedData"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un dato a fasi temporali."
type: docs
weight: 320
url: /it/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Rappresenta un dato a fasi temporali.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Crea e inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata) per dati temporizzati basati sul costo. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Crea e inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata) per dati temporizzati basati sul costo. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Crea e inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata) per dati temporizzati basati sull'unità di un'assegnazione di una risorsa materiale. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Crea e inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata) per dati temporizzati basati sul lavoro. |
| [getFinish()](#getFinish--) | Restituisce la data di fine di un periodo di dati temporizzati. |
| [getStart()](#getStart--) | Restituisce la data di inizio di un periodo di dati temporizzati. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Restituisce il tipo di un dato temporizzato. |
| [getUid()](#getUid--) | Restituisce l'identificatore univoco di un dato temporizzato |
| [getUnit()](#getUnit--) | Restituisce l'unità di tempo di un periodo di dati temporizzati. |
| [getValue()](#getValue--) | Restituisce il valore per unità di tempo di un periodo di dati temporizzati. |
| [getValueToCost()](#getValueToCost--) | Restituisce l'istanza `double` che rappresenta il valore stringa di questo oggetto. |
| [getValueToDuration()](#getValueToDuration--) | Restituisce l'istanza double che rappresenta il valore stringa di questo oggetto. |
| [getValueToUnits()](#getValueToUnits--) | Restituisce l'istanza `double` che rappresenta il valore stringa di questo oggetto per dati temporizzati basati sull'unità. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Imposta la data di fine di un periodo di dati temporizzati. |
| [setStart(Date value)](#setStart-java.util.Date-) | Imposta la data di inizio di un periodo di dati temporizzati. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Imposta il tipo di un dato temporizzato. |
| [setUid(int value)](#setUid-int-) | Imposta l'identificatore univoco di un dato temporizzato |
| [setUnit(byte value)](#setUnit-byte-) | Imposta l'unità di tempo di un periodo di dati temporizzati. |
| [setValue(String value)](#setValue-java.lang.String-) | Imposta il valore per unità di tempo di un periodo di dati temporizzati. |
| [setValueToCost(double value)](#setValueToCost-double-) | Istanza `double` che rappresenta il valore stringa di questo oggetto. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata).

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Crea e inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata) per dati temporizzati basati sul costo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | int | UID dell'attività. |
| inizio | java.util.Date | data-ora di inizio. |
| fine | java.util.Date | Data-ora di fine. |
| valore | double | Valore del costo. |
| type | byte | Tipo di dato temporizzato. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Crea e inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata) per dati temporizzati basati sul costo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | int | UID dell'attività. |
| inizio | java.util.Date | data-ora di inizio. |
| fine | java.util.Date | Data-ora di fine. |
| valore | double | Valore del costo. |
| timeUnit | byte | Tipo di unità di tempo. |
| type | byte | Tipo di dato temporizzato. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Crea e inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata) per dati temporizzati basati sull'unità di un'assegnazione di una risorsa materiale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | int | UID dell'attività. |
| inizio | java.util.Date | Data e ora di inizio. |
| fine | java.util.Date | Data-ora di fine. |
| unità | double | Numero di unità. |
| type | byte | Tipo di dato temporizzato. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Crea e inizializza una nuova istanza della classe [TimephasedData](../../com.aspose.tasks/timephaseddata) per dati temporizzati basati sul lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | int | UID dell'attività. |
| inizio | java.util.Date | data-ora di inizio. |
| fine | java.util.Date | Data-ora di fine. |
| valore | double | Valore dell'intervallo di tempo. |
| timeUnit | byte | Tipo di unità di tempo. |
| type | byte | Tipo di dato temporizzato. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Restituisce la data di fine di un periodo di dati temporizzati.

**Returns:**
java.util.Date - la data di fine di un periodo di dati a fasi temporali.
### getStart() {#getStart--}
```
public final Date getStart()
```


Restituisce la data di inizio di un periodo di dati temporizzati.

**Returns:**
java.util.Date - la data di inizio di un periodo di dati a fasi temporali.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Restituisce il tipo di un dato temporizzato.

--------------------

`Value`([getValue()](../../com.aspose/tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose/tasks/timephaseddata\#setValue-String-)) la proprietà verrà cancellata, se non è adatta al tipo specificato qui.

**Returns:**
byte - il tipo di un dato a fasi temporali.
### getUid() {#getUid--}
```
public final int getUid()
```


Restituisce l'identificatore univoco di un dato temporizzato

**Returns:**
int - l'identificatore univoco di un dato a fasi temporali
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Restituisce l'unità di tempo di un periodo di dati temporizzati.

**Returns:**
byte - l'unità di tempo di un periodo di dati a fasi temporali.
### getValue() {#getValue--}
```
public final String getValue()
```


Restituisce il valore per unità di tempo di un periodo di dati temporizzati.

**Returns:**
java.lang.String - il valore per unità di tempo per un periodo di dati a fasi temporali.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


Restituisce l'istanza `double` che rappresenta il valore stringa di questo oggetto.

**Returns:**
double - una rappresentazione in virgola mobile dell'oggetto.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


Restituisce l'istanza double che rappresenta il valore stringa di questo oggetto.

**Returns:**
double - una rappresentazione dell'intervallo di tempo dell'oggetto.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Restituisce l'istanza `double` che rappresenta il valore stringa di questo oggetto per dati temporizzati basati sull'unità.

**Returns:**
double - una rappresentazione in virgola mobile di questo oggetto.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Imposta la data di fine di un periodo di dati temporizzati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la data di fine di un periodo di dati a fasi temporali. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Imposta la data di inizio di un periodo di dati temporizzati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la data di inizio di un periodo di dati a fasi temporali. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Imposta il tipo di un dato temporizzato.

--------------------

`Value`([getValue()](../../com.aspose/tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose/tasks/timephaseddata\#setValue-String-)) la proprietà verrà cancellata, se non è adatta al tipo specificato qui.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte | il tipo di un dato a fasi temporali. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Imposta l'identificatore univoco di un dato temporizzato

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'identificatore univoco di un dato a fasi temporali |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Imposta l'unità di tempo di un periodo di dati temporizzati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte | l'unità di tempo di un periodo di dati a fasi temporali. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Imposta il valore per unità di tempo di un periodo di dati temporizzati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il valore per unità di tempo per un periodo di dati a fasi temporali. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


Istanza `double` che rappresenta il valore stringa di questo oggetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | Istanza `double` che rappresenta il valore stringa di questo oggetto. |

