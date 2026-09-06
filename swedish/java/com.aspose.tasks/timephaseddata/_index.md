---
title: "TimephasedData"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar tidsfasad data."
type: docs
weight: 320
url: /sv/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Representerar tidsfasad data.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Skapar och initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata) för kostnadsbaserad tidsfasad data. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Skapar och initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata) för kostnadsbaserad tidsfasad data. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Skapar och initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata) för enhetsbaserad tidsfasad data för en tilldelning av en materialresurs. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Skapar och initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata) för arbetsbaserad tidsfasad data. |
| [getFinish()](#getFinish--) | Hämtar slutdatumet för en tidsfasad dataperiod. |
| [getStart()](#getStart--) | Hämtar startdatumet för en tidsfasad dataperiod. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Hämtar typen av en tidsfasad data. |
| [getUid()](#getUid--) | Hämtar den unika identifieraren för en tidsfasad data |
| [getUnit()](#getUnit--) | Hämtar tidsenheten för en tidsfasad dataperiod. |
| [getValue()](#getValue--) | Hämtar värdet per tidsenhet för en tidsfasad dataperiod. |
| [getValueToCost()](#getValueToCost--) | Hämtar `double`-instans som representerar strängvärdet för detta objekt. |
| [getValueToDuration()](#getValueToDuration--) | Hämtar double-instans som representerar strängvärdet för detta objekt. |
| [getValueToUnits()](#getValueToUnits--) | Hämtar `double`-instans som representerar strängvärdet för detta objekt för enhetsbaserad tidsfasad data. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Ställer in slutdatumet för en tidsfasad dataperiod. |
| [setStart(Date value)](#setStart-java.util.Date-) | Ställer in startdatumet för en tidsfasad dataperiod. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Ställer in typen av en tidsfasad data. |
| [setUid(int value)](#setUid-int-) | Ställer in den unika identifieraren för en tidsfasad data |
| [setUnit(byte value)](#setUnit-byte-) | Ställer in tidsenheten för en tidsfasad dataperiod. |
| [setValue(String value)](#setValue-java.lang.String-) | Ställer in värdet per tidsenhet för en tidsfasad dataperiod. |
| [setValueToCost(double value)](#setValueToCost-double-) | `double`-instans som representerar strängvärdet för detta objekt. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata).

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Skapar och initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata) för kostnadsbaserad tidsfasad data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | int | UID för uppgiften. |
| start | java.util.Date | startdatum‑tid. |
| slut | java.util.Date | slutdatum‑tid. |
| värde | double | Kostnadsvärde. |
| typ | byte | Tidsfasad datatyp. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Skapar och initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata) för kostnadsbaserad tidsfasad data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | int | UID för uppgiften. |
| start | java.util.Date | startdatum‑tid. |
| slut | java.util.Date | slutdatum‑tid. |
| värde | double | Kostnadsvärde. |
| tidsenhet | byte | Tidsenhetstyp. |
| typ | byte | Tidsfasad datatyp. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Skapar och initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata) för enhetsbaserad tidsfasad data för en tilldelning av en materialresurs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | int | UID för uppgiften. |
| start | java.util.Date | Startdatum‑tid. |
| slut | java.util.Date | slutdatum‑tid. |
| enheter | double | Antal enheter. |
| typ | byte | Tidsfasad datatyp. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Skapar och initierar en ny instans av klassen [TimephasedData](../../com.aspose.tasks/timephaseddata) för arbetsbaserad tidsfasad data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | int | UID för uppgiften. |
| start | java.util.Date | startdatum‑tid. |
| slut | java.util.Date | slutdatum‑tid. |
| värde | double | Tidsintervallvärde. |
| tidsenhet | byte | Tidsenhetstyp. |
| typ | byte | Tidsfasad datatyp. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Hämtar slutdatumet för en tidsfasad dataperiod.

**Returns:**
java.util.Date - slutdatumet för en tidsfasad dataperiod.
### getStart() {#getStart--}
```
public final Date getStart()
```


Hämtar startdatumet för en tidsfasad dataperiod.

**Returns:**
java.util.Date - startdatumet för en tidsfasad dataperiod.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Hämtar typen av en tidsfasad data.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) egenskap kommer att rensas om den inte är lämplig för den typ som specificeras här.

**Returns:**
byte - typen av en tidsfasad data.
### getUid() {#getUid--}
```
public final int getUid()
```


Hämtar den unika identifieraren för en tidsfasad data

**Returns:**
int - den unika identifieraren för en tidsfasad data
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Hämtar tidsenheten för en tidsfasad dataperiod.

**Returns:**
byte - tidsenheten för en tidsfasad dataperiod.
### getValue() {#getValue--}
```
public final String getValue()
```


Hämtar värdet per tidsenhet för en tidsfasad dataperiod.

**Returns:**
java.lang.String - värdet per tidsenhet för en tidsfasad dataperiod.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


Hämtar `double`-instans som representerar strängvärdet för detta objekt.

**Returns:**
double - en flyttalsrepresentation av objektet.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


Hämtar double-instans som representerar strängvärdet för detta objekt.

**Returns:**
double - en tidsintervallrepresentation av objektet.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Hämtar `double`-instans som representerar strängvärdet för detta objekt för enhetsbaserad tidsfasad data.

**Returns:**
double - en flyttalsrepresentation av detta objekt.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Ställer in slutdatumet för en tidsfasad dataperiod.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | slutdatumet för en tidsfasad dataperiod. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Ställer in startdatumet för en tidsfasad dataperiod.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | startdatumet för en tidsfasad dataperiod. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Ställer in typen av en tidsfasad data.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) egenskap kommer att rensas om den inte är lämplig för den typ som specificeras här.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte | typen av en tidsfasad data. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Ställer in den unika identifieraren för en tidsfasad data

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | den unika identifieraren för en tidsfasad data |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Ställer in tidsenheten för en tidsfasad dataperiod.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte | tidsenheten för en tidsfasad dataperiod. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Ställer in värdet per tidsenhet för en tidsfasad dataperiod.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | värdet per tidsenhet för en tidsfasad dataperiod. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


`double`-instans som representerar strängvärdet för detta objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | `double`-instans som representerar strängvärdet för detta objekt. |

