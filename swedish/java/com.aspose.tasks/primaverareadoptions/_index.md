---
title: "PrimaveraReadOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när Primavera Xml- eller Primavera Xer-filer läses."
type: docs
weight: 206
url: /sv/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Tillåter att ange ytterligare alternativ när Primavera Xml- eller Primavera Xer-filer läses.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Initierar en ny instans av klassen [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Hämtar en flagga som anger om de ursprungliga unika identifierarna för enheter ska bevaras. |
| [getProjectUid()](#getProjectUid--) | Hämtar UID för ett projekt att läsa från en fil som innehåller flera projekt. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Hämtar en flagga som anger om baslinjeprojekt ska läsas in. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | Anger beteendet som används för att bearbeta uppgifter med odefinierade begränsningar lästa från XER-format. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Ställer in en flagga som anger om de ursprungliga unika identifierarna för enheter ska bevaras. |
| [setProjectUid(int value)](#setProjectUid-int-) | Ställer in UID för ett projekt att läsa från en fil som innehåller flera projekt. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Ställer in en flagga som anger om baslinjeprojekt ska läsas in. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | Anger beteendet som används för att bearbeta uppgifter med odefinierade begränsningar lästa från XER-format. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Initierar en ny instans av klassen [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions).

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Hämtar en flagga som anger om de ursprungliga unika identifierarna för enheter ska bevaras.

**Returns:**
boolean - en flagga som anger om de ursprungliga unika identifierarna för enheter ska bevaras.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Hämtar UID för ett projekt att läsa från en fil som innehåller flera projekt.

**Returns:**
int - UID för ett projekt att läsa från en fil som innehåller flera projekt.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Hämtar en flagga som anger om baslinjeprojekt ska läsas in. Standardvärdet är true.

--------------------

Flaggan är tillämplig på Primavera XML-filer som innehåller baslinjeprojekt (baslinjer stöds inte av XER-format). Alternativet kan sättas till false för att snabba upp inläsning av ett stort projekt med baslinjer när baslinjedata inte behövs.

**Returns:**
boolean - en flagga som anger om baslinjeprojekt ska läsas in.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


Anger beteendet som används för att bearbeta uppgifter med odefinierade begränsningar lästa från XER-format.

**Returns:**
int - beteendet som används för att bearbeta uppgifter med odefinierade begränsningar lästa från XER-format.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Ställer in en flagga som anger om de ursprungliga unika identifierarna för enheter ska bevaras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | en flagga som anger om de ursprungliga unika identifierarna för enheter ska bevaras. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Ställer in UID för ett projekt att läsa från en fil som innehåller flera projekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | UID för ett projekt att läsa från en fil som innehåller flera projekt. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Ställer in en flagga som anger om baslinjeprojekt ska laddas. Standardvärdet är true.

--------------------

Flaggan är tillämplig på Primavera XML-filer som innehåller baslinjeprojekt (baslinjer stöds inte av XER-format). Alternativet kan sättas till false för att snabba upp inläsning av ett stort projekt med baslinjer när baslinjedata inte behövs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | en flagga som anger om baslinjeprojekt ska laddas. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


Anger beteendet som används för att bearbeta uppgifter med odefinierade begränsningar lästa från XER-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | beteendet som används för att bearbeta uppgifter med odefinierade begränsningar lästa från XER-format. |

