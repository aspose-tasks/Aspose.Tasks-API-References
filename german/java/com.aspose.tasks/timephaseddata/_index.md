---
title: "TimephasedData"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt zeitphasenbezogene Daten dar."
type: docs
weight: 320
url: /de/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Stellt zeitphasenbezogene Daten dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Erstellt und initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata) für kostenbasierte zeitphasenbezogene Daten. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Erstellt und initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata) für kostenbasierte zeitphasenbezogene Daten. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Erstellt und initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata) für einheitenbasierte zeitphasenbezogene Daten einer Zuweisung einer Materialressource. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Erstellt und initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata) für arbeitsbasierte zeitphasenbezogene Daten. |
| [getFinish()](#getFinish--) | Liefert das Enddatum eines zeitphasenbezogenen Datenzeitraums. |
| [getStart()](#getStart--) | Liefert das Startdatum eines zeitphasenbezogenen Datenzeitraums. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Liefert den Typ einer zeitphasenbezogenen Daten. |
| [getUid()](#getUid--) | Liefert die eindeutige Kennung einer zeitphasenbezogenen Daten. |
| [getUnit()](#getUnit--) | Liefert die Zeiteinheit eines zeitphasenbezogenen Datenzeitraums. |
| [getValue()](#getValue--) | Liefert den Wert pro Zeiteinheit für einen zeitphasenbezogenen Datenzeitraum. |
| [getValueToCost()](#getValueToCost--) | Liefert die `double`-Instanz, die den Zeichenkettenwert dieses Objekts darstellt. |
| [getValueToDuration()](#getValueToDuration--) | Liefert die double-Instanz, die den Zeichenkettenwert dieses Objekts darstellt. |
| [getValueToUnits()](#getValueToUnits--) | Liefert die `double`-Instanz, die den Zeichenkettenwert dieses Objekts für einheitenbasierte zeitphasenbezogene Daten darstellt. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Setzt das Enddatum eines zeitphasenbezogenen Datenzeitraums. |
| [setStart(Date value)](#setStart-java.util.Date-) | Setzt das Startdatum eines zeitphasenbezogenen Datenzeitraums. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Setzt den Typ einer zeitphasenbezogenen Daten. |
| [setUid(int value)](#setUid-int-) | Setzt den eindeutigen Bezeichner einer zeitphasenbezogenen Daten. |
| [setUnit(byte value)](#setUnit-byte-) | Setzt die Zeiteinheit eines zeitphasenbezogenen Datenzeitraums. |
| [setValue(String value)](#setValue-java.lang.String-) | Setzt den Wert pro Zeiteinheit für einen zeitphasenbezogenen Datenzeitraum. |
| [setValueToCost(double value)](#setValueToCost-double-) | `double`-Instanz, die den Zeichenkettenwert dieses Objekts darstellt. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata).

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Erstellt und initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata) für kostenbasierte zeitphasenbezogene Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | int | UID der Aufgabe. |
| start | java.util.Date | Start-Datum-Uhrzeit. |
| Abschluss | java.util.Date | Ende-Datum-Uhrzeit. |
| Wert | double | Kostenwert. |
| Typ | byte | Zeitphasenbezogener Datentyp. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Erstellt und initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata) für kostenbasierte zeitphasenbezogene Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | int | UID der Aufgabe. |
| start | java.util.Date | Start-Datum-Uhrzeit. |
| Abschluss | java.util.Date | Ende-Datum-Uhrzeit. |
| Wert | double | Kostenwert. |
| timeUnit | byte | Zeiteinheitstyp. |
| Typ | byte | Zeitphasenbezogener Datentyp. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Erstellt und initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata) für einheitenbasierte zeitphasenbezogene Daten einer Zuweisung einer Materialressource.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | int | UID der Aufgabe. |
| start | java.util.Date | Start-Datum-Uhrzeit. |
| Abschluss | java.util.Date | Ende-Datum-Uhrzeit. |
| Einheiten | double | Anzahl der Einheiten. |
| Typ | byte | Zeitphasenbezogener Datentyp. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Erstellt und initialisiert eine neue Instanz der Klasse [TimephasedData](../../com.aspose.tasks/timephaseddata) für arbeitsbasierte zeitphasenbezogene Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | int | UID der Aufgabe. |
| start | java.util.Date | Start-Datum-Uhrzeit. |
| Abschluss | java.util.Date | Ende-Datum-Uhrzeit. |
| Wert | double | Zeitspannenwert. |
| timeUnit | byte | Zeiteinheitstyp. |
| Typ | byte | Zeitphasenbezogener Datentyp. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Liefert das Enddatum eines zeitphasenbezogenen Datenzeitraums.

**Returns:**
java.util.Date - das Enddatum eines zeitphasenbezogenen Datenzeitraums.
### getStart() {#getStart--}
```
public final Date getStart()
```


Liefert das Startdatum eines zeitphasenbezogenen Datenzeitraums.

**Returns:**
java.util.Date - das Startdatum eines zeitphasenbezogenen Datenzeitraums.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Liefert den Typ einer zeitphasenbezogenen Daten.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) Eigenschaft wird gelöscht, wenn sie nicht zum hier angegebenen Typ passt.

**Returns:**
byte - der Typ einer zeitphasenbezogenen Daten.
### getUid() {#getUid--}
```
public final int getUid()
```


Liefert die eindeutige Kennung einer zeitphasenbezogenen Daten.

**Returns:**
int - der eindeutige Bezeichner einer zeitphasenbezogenen Daten
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Liefert die Zeiteinheit eines zeitphasenbezogenen Datenzeitraums.

**Returns:**
byte - die Zeiteinheit eines zeitphasenbezogenen Datenzeitraums.
### getValue() {#getValue--}
```
public final String getValue()
```


Liefert den Wert pro Zeiteinheit für einen zeitphasenbezogenen Datenzeitraum.

**Returns:**
java.lang.String - der Wert pro Zeiteinheit für einen zeitlich gestuften Datenabschnitt.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


Liefert die `double`-Instanz, die den Zeichenkettenwert dieses Objekts darstellt.

**Returns:**
double - eine Gleitkommadarstellung des Objekts.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


Liefert die double-Instanz, die den Zeichenkettenwert dieses Objekts darstellt.

**Returns:**
double - eine Zeitspannen-Darstellung des Objekts.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Liefert die `double`-Instanz, die den Zeichenkettenwert dieses Objekts für einheitenbasierte zeitphasenbezogene Daten darstellt.

**Returns:**
double - eine Gleitkommadarstellung dieses Objekts.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Setzt das Enddatum eines zeitphasenbezogenen Datenzeitraums.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das Enddatum eines zeitlich gestuften Datenabschnitts. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Setzt das Startdatum eines zeitphasenbezogenen Datenzeitraums.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das Startdatum eines zeitlich gestuften Datenabschnitts. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Setzt den Typ einer zeitphasenbezogenen Daten.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) Eigenschaft wird gelöscht, wenn sie nicht zum hier angegebenen Typ passt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte | der Typ einer zeitlich gestuften Daten. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Setzt den eindeutigen Bezeichner einer zeitphasenbezogenen Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der eindeutige Bezeichner einer zeitlich gestuften Daten |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Setzt die Zeiteinheit eines zeitphasenbezogenen Datenzeitraums.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte | die Zeiteinheit eines zeitlich gestuften Datenabschnitts. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Setzt den Wert pro Zeiteinheit für einen zeitphasenbezogenen Datenzeitraum.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der Wert pro Zeiteinheit für einen zeitlich gestuften Datenabschnitt. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


`double`-Instanz, die den Zeichenkettenwert dieses Objekts darstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | `double`-Instanz, die den Zeichenkettenwert dieses Objekts darstellt. |

