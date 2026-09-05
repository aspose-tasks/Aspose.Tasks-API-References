---
title: "PrimaveraReadOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe extra opties op te geven bij het lezen van Primavera-Xml- of Primavera-Xer-bestanden."
type: docs
weight: 206
url: /nl/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Staat toe extra opties op te geven bij het lezen van Primavera-Xml- of Primavera-Xer-bestanden.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Initialiseert een nieuw exemplaar van de [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Haalt een vlag op die aangeeft of originele unieke identifiers van entiteiten behouden moeten blijven. |
| [getProjectUid()](#getProjectUid--) | Haalt de UID op van een project om te lezen uit een bestand dat meerdere projecten bevat. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Haalt een vlag op die aangeeft of baselineprojecten geladen moeten worden. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | Specificeert het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen, gelezen uit XER-indeling, te verwerken. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Stelt een vlag in die aangeeft of originele unieke identifiers van entiteiten behouden moeten blijven. |
| [setProjectUid(int value)](#setProjectUid-int-) | Stelt de UID in van een project om te lezen uit een bestand dat meerdere projecten bevat. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Stelt een vlag in die aangeeft of baselineprojecten geladen moeten worden. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | Specificeert het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen, gelezen uit XER-indeling, te verwerken. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Initialiseert een nieuw exemplaar van de [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) klasse.

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Haalt een vlag op die aangeeft of originele unieke identifiers van entiteiten behouden moeten blijven.

**Returns:**
boolean - een vlag die aangeeft of originele unieke identifiers van entiteiten behouden moeten blijven.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Haalt de UID op van een project om te lezen uit een bestand dat meerdere projecten bevat.

**Returns:**
int - de UID van een project om te lezen uit een bestand dat meerdere projecten bevat.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Haalt een vlag op die aangeeft of baselineprojecten geladen moeten worden. De standaardwaarde is true.

--------------------

De vlag is van toepassing op Primavera XML-bestanden die baselineprojecten bevatten (baselineprojecten worden niet ondersteund door XER-indeling). De optie kan op false worden gezet om het laden van een groot project met baselineprojecten te versnellen wanneer baselinegegevens niet nodig zijn.

**Returns:**
boolean - een vlag die aangeeft of baselineprojecten geladen moeten worden.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


Specificeert het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen, gelezen uit XER-indeling, te verwerken.

**Returns:**
int - het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen, gelezen uit XER-indeling, te verwerken.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Stelt een vlag in die aangeeft of originele unieke identifiers van entiteiten behouden moeten blijven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een vlag die aangeeft of originele unieke identifiers van entiteiten behouden moeten blijven. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Stelt de UID in van een project om te lezen uit een bestand dat meerdere projecten bevat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de UID van een project om te lezen uit een bestand dat meerdere projecten bevat. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Stelt een vlag in die aangeeft of baselineprojecten moeten worden geladen. De standaardwaarde is true.

--------------------

De vlag is van toepassing op Primavera XML-bestanden die baselineprojecten bevatten (baselineprojecten worden niet ondersteund door XER-indeling). De optie kan op false worden gezet om het laden van een groot project met baselineprojecten te versnellen wanneer baselinegegevens niet nodig zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een vlag die aangeeft of baselineprojecten moeten worden geladen. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


Specificeert het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen, gelezen uit XER-indeling, te verwerken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen, gelezen uit XER-indeling, te verwerken. |

