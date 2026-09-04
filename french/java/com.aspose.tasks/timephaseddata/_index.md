---
title: "TimephasedData"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une donnée à phase temporelle."
type: docs
weight: 320
url: /fr/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Représente une donnée à phase temporelle.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Crée et initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata) pour les données temporelles basées sur les coûts. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Crée et initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata) pour les données temporelles basées sur les coûts. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Crée et initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata) pour les données temporelles basées sur l'unité d'une affectation d'une ressource matérielle. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Crée et initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata) pour les données temporelles basées sur le travail. |
| [getFinish()](#getFinish--) | Obtient la date de fin d'une période de données temporelles. |
| [getStart()](#getStart--) | Obtient la date de début d'une période de données temporelles. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Obtient le type d'une donnée temporelle. |
| [getUid()](#getUid--) | Obtient l'identifiant unique d'une donnée temporelle |
| [getUnit()](#getUnit--) | Obtient l'unité de temps d'une période de données temporelles. |
| [getValue()](#getValue--) | Obtient la valeur par unité de temps pour une période de données temporelles. |
| [getValueToCost()](#getValueToCost--) | Obtient l'instance `double` qui représente la valeur chaîne de cet objet. |
| [getValueToDuration()](#getValueToDuration--) | Obtient l'instance double qui représente la valeur chaîne de cet objet. |
| [getValueToUnits()](#getValueToUnits--) | Obtient l'instance `double` qui représente la valeur chaîne de cet objet pour les données temporelles basées sur l'unité. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Définit la date de fin d'une période de données temporelles. |
| [setStart(Date value)](#setStart-java.util.Date-) | Définit la date de début d'une période de données temporelles. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Définit le type d'une donnée temporelle. |
| [setUid(int value)](#setUid-int-) | Définit l'identifiant unique d'une donnée temporelle |
| [setUnit(byte value)](#setUnit-byte-) | Définit l'unité de temps d'une période de données temporelles. |
| [setValue(String value)](#setValue-java.lang.String-) | Définit la valeur par unité de temps pour une période de données temporelles. |
| [setValueToCost(double value)](#setValueToCost-double-) | Instance `double` qui représente la valeur chaîne de cet objet. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata).

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Crée et initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata) pour les données temporelles basées sur les coûts.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | int | UID de la tâche. |
| début | java.util.Date | date-heure de début. |
| fin | java.util.Date | Date-heure de fin. |
| valeur | double | Valeur du coût. |
| type | byte | Type de données temporelles. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Crée et initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata) pour les données temporelles basées sur les coûts.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | int | UID de la tâche. |
| début | java.util.Date | date-heure de début. |
| fin | java.util.Date | Date-heure de fin. |
| valeur | double | Valeur du coût. |
| timeUnit | byte | Type d'unité de temps. |
| type | byte | Type de données temporelles. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Crée et initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata) pour les données temporelles basées sur l'unité d'une affectation d'une ressource matérielle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | int | UID de la tâche. |
| début | java.util.Date | Date et heure de début. |
| fin | java.util.Date | Date-heure de fin. |
| unités | double | Nombre d'unités. |
| type | byte | Type de données temporelles. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Crée et initialise une nouvelle instance de la classe [TimephasedData](../../com.aspose.tasks/timephaseddata) pour les données temporelles basées sur le travail.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | int | UID de la tâche. |
| début | java.util.Date | date-heure de début. |
| fin | java.util.Date | Date-heure de fin. |
| valeur | double | Valeur de la durée. |
| timeUnit | byte | Type d'unité de temps. |
| type | byte | Type de données temporelles. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Obtient la date de fin d'une période de données temporelles.

**Returns:**
java.util.Date - la date de fin d'une période de données à phases temporelles.
### getStart() {#getStart--}
```
public final Date getStart()
```


Obtient la date de début d'une période de données temporelles.

**Returns:**
java.util.Date - la date de début d'une période de données à phases temporelles.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Obtient le type d'une donnée temporelle.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) la propriété sera effacée, si elle n'est pas adaptée au type spécifié ici.

**Returns:**
byte - le type d'une donnée à phases temporelles.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtient l'identifiant unique d'une donnée temporelle

**Returns:**
int - l'identifiant unique d'une donnée à phases temporelles
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Obtient l'unité de temps d'une période de données temporelles.

**Returns:**
byte - l'unité de temps d'une période de données à phases temporelles.
### getValue() {#getValue--}
```
public final String getValue()
```


Obtient la valeur par unité de temps pour une période de données temporelles.

**Returns:**
java.lang.String - la valeur par unité de temps pour une période de données à phases temporelles.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


Obtient l'instance `double` qui représente la valeur chaîne de cet objet.

**Returns:**
double - une représentation en virgule flottante de l'objet.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


Obtient l'instance double qui représente la valeur chaîne de cet objet.

**Returns:**
double - une représentation de la durée de l'objet.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Obtient l'instance `double` qui représente la valeur chaîne de cet objet pour les données temporelles basées sur l'unité.

**Returns:**
double - une représentation en virgule flottante de cet objet.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Définit la date de fin d'une période de données temporelles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la date de fin d'une période de données à phases temporelles. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Définit la date de début d'une période de données temporelles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la date de début d'une période de données à phases temporelles. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Définit le type d'une donnée temporelle.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) la propriété sera effacée, si elle n'est pas adaptée au type spécifié ici.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte | le type d'une donnée à phases temporelles. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Définit l'identifiant unique d'une donnée temporelle

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'identifiant unique d'une donnée à phases temporelles |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Définit l'unité de temps d'une période de données temporelles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte | l'unité de temps d'une période de données à phases temporelles. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Définit la valeur par unité de temps pour une période de données temporelles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la valeur par unité de temps pour une période de données à phases temporelles. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


Instance `double` qui représente la valeur chaîne de cet objet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | Instance `double` qui représente la valeur chaîne de cet objet. |

