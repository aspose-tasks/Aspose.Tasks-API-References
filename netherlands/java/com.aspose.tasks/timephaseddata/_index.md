---
title: "TimephasedData"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een tijdgephaseerde gegevens voor."
type: docs
weight: 320
url: /nl/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Stelt een tijdgephaseerde gegevens voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Initialiseert een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Maakt een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse aan en initialiseert deze voor kosten-gebaseerde tijdsfasegegevens. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Maakt een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse aan en initialiseert deze voor kosten-gebaseerde tijdsfasegegevens. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Maakt een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse aan en initialiseert deze voor eenheid-gebaseerde tijdsfasegegevens van een toewijzing van een materiële resource. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Maakt een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse aan en initialiseert deze voor werk-gebaseerde tijdsfasegegevens. |
| [getFinish()](#getFinish--) | Haalt de einddatum op van een tijdsfasegegevensperiode. |
| [getStart()](#getStart--) | Haalt de startdatum op van een tijdsfasegegevensperiode. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Haalt het type op van een tijdsfasegegevens. |
| [getUid()](#getUid--) | Haalt de unieke identifier op van een tijdsfasegegevens |
| [getUnit()](#getUnit--) | Haalt de tijdseenheid op van een tijdsfasegegevensperiode. |
| [getValue()](#getValue--) | Haalt de waarde per tijdseenheid op voor een tijdsfasegegevensperiode. |
| [getValueToCost()](#getValueToCost--) | Haalt de `double`-instantie op die de tekenreekswaarde van dit object vertegenwoordigt. |
| [getValueToDuration()](#getValueToDuration--) | Haalt double instantie op die de tekenreekswaarde van dit object vertegenwoordigt. |
| [getValueToUnits()](#getValueToUnits--) | Haalt de `double`-instantie op die de tekenreekswaarde van dit object vertegenwoordigt voor eenheid-gebaseerde tijdsfasegegevens. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Stelt de einddatum in van een tijdsfasegegevensperiode. |
| [setStart(Date value)](#setStart-java.util.Date-) | Stelt de startdatum in van een tijdsfasegegevensperiode. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Stelt het type in van een tijdsfasegegevens. |
| [setUid(int value)](#setUid-int-) | Stelt de unieke identifier in van een tijdsfasegegevens |
| [setUnit(byte value)](#setUnit-byte-) | Stelt de tijdseenheid in van een tijdsfasegegevensperiode. |
| [setValue(String value)](#setValue-java.lang.String-) | Stelt de waarde per tijdseenheid in voor een tijdsfasegegevensperiode. |
| [setValueToCost(double value)](#setValueToCost-double-) | `double`-instantie die de tekenreekswaarde van dit object vertegenwoordigt. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Initialiseert een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse.

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Maakt een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse aan en initialiseert deze voor kosten-gebaseerde tijdsfasegegevens.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uid | int | UID van de taak. |
| start | java.util.Date | start datum-tijd. |
| einde | java.util.Date | Finish datum-tijd. |
| waarde | double | Kostenwaarde. |
| type | byte | Tijdsfasegegevenstype. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Maakt een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse aan en initialiseert deze voor kosten-gebaseerde tijdsfasegegevens.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uid | int | UID van de taak. |
| start | java.util.Date | start datum-tijd. |
| einde | java.util.Date | Finish datum-tijd. |
| waarde | double | Kostenwaarde. |
| timeUnit | byte | Tijdseenheidstype. |
| type | byte | Tijdsfasegegevenstype. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Maakt een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse aan en initialiseert deze voor eenheid-gebaseerde tijdsfasegegevens van een toewijzing van een materiële resource.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uid | int | UID van de taak. |
| start | java.util.Date | Start datum‑tijd. |
| einde | java.util.Date | Finish datum-tijd. |
| eenheden | double | Aantal eenheden. |
| type | byte | Tijdsfasegegevenstype. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Maakt een nieuw exemplaar van de [TimephasedData](../../com.aspose.tasks/timephaseddata) klasse aan en initialiseert deze voor werk-gebaseerde tijdsfasegegevens.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uid | int | UID van de taak. |
| start | java.util.Date | start datum-tijd. |
| einde | java.util.Date | Finish datum-tijd. |
| waarde | double | Tijdsduurwaarde. |
| timeUnit | byte | Tijdseenheidstype. |
| type | byte | Tijdsfasegegevenstype. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Haalt de einddatum op van een tijdsfasegegevensperiode.

**Returns:**
java.util.Date - de einddatum van een tijdsfasegegevensperiode.
### getStart() {#getStart--}
```
public final Date getStart()
```


Haalt de startdatum op van een tijdsfasegegevensperiode.

**Returns:**
java.util.Date - de startdatum van een tijdsfasegegevensperiode.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Haalt het type op van een tijdsfasegegevens.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) eigenschap wordt gewist als deze niet geschikt is voor het hier gespecificeerde type.

**Returns:**
byte - het type van een tijdsfasegegevens.
### getUid() {#getUid--}
```
public final int getUid()
```


Haalt de unieke identifier op van een tijdsfasegegevens

**Returns:**
int - de unieke identifier van een tijdsfasegegevens.
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Haalt de tijdseenheid op van een tijdsfasegegevensperiode.

**Returns:**
byte - de tijdseenheid van een tijdsfasegegevensperiode.
### getValue() {#getValue--}
```
public final String getValue()
```


Haalt de waarde per tijdseenheid op voor een tijdsfasegegevensperiode.

**Returns:**
java.lang.String - de waarde per tijdseenheid voor een tijdsfasegegevensperiode.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


Haalt de `double`-instantie op die de tekenreekswaarde van dit object vertegenwoordigt.

**Returns:**
double - een zwevendekommagetalrepresentatie van het object.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


Haalt double instantie op die de tekenreekswaarde van dit object vertegenwoordigt.

**Returns:**
double - een tijdsduurrepresentatie van het object.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Haalt de `double`-instantie op die de tekenreekswaarde van dit object vertegenwoordigt voor eenheid-gebaseerde tijdsfasegegevens.

**Returns:**
double - een zwevendekommagetalrepresentatie van dit object.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Stelt de einddatum in van een tijdsfasegegevensperiode.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de einddatum van een tijdsfasegegevensperiode. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Stelt de startdatum in van een tijdsfasegegevensperiode.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de startdatum van een tijdsfasegegevensperiode. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Stelt het type in van een tijdsfasegegevens.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) eigenschap wordt gewist als deze niet geschikt is voor het hier gespecificeerde type.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | byte | het type van een tijdsfasegegevens. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Stelt de unieke identifier in van een tijdsfasegegevens

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de unieke identifier van een tijdsfasegegevens |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Stelt de tijdseenheid in van een tijdsfasegegevensperiode.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | byte | de tijdseenheid van een tijdsfasegegevensperiode. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Stelt de waarde per tijdseenheid in voor een tijdsfasegegevensperiode.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de waarde per tijdseenheid voor een tijdsfasegegevensperiode. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


`double`-instantie die de tekenreekswaarde van dit object vertegenwoordigt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | `double`-instantie die de tekenreekswaarde van dit object vertegenwoordigt. |

