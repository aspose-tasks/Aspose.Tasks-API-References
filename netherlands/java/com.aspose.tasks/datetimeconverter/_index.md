---
title: "DateTimeConverter"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Vertegenwoordigt een converter voor het omzetten van een datum naar een tekenreeks in weergave‑tijdschaal‑lagen."
type: docs
weight: 70
url: /nl/java/com.aspose.tasks/datetimeconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class DateTimeConverter extends System.MulticastDelegate
```

Vertegenwoordigt een converter voor het omzetten van een datum naar een tekenreeks in weergave‑tijdschaal‑lagen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DateTimeConverter()](#DateTimeConverter--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [invoke(Date date)](#invoke-java.util.Date-) | Stelt een convertermethode voor om een datum naar een tekenreeks te converteren in weergave-tijdschalenniveaus. |
### DateTimeConverter() {#DateTimeConverter--}
```
public DateTimeConverter()
```


### invoke(Date date) {#invoke-java.util.Date-}
```
public abstract String invoke(Date date)
```


Stelt een convertermethode voor om een datum naar een tekenreeks te converteren in weergave-tijdschalenniveaus.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| datum | java.util.Date | de instantie van de `java.util.Date`-klasse om te converteren naar een tekenreeks. |

**Returns:**
java.lang.String - de tekenreeksrepresentatie van de opgegeven datum.
