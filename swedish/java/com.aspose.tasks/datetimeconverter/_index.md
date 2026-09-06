---
title: "DateTimeConverter"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en konverterare för att omvandla datum till sträng i visningsnivåer för tidslinjen."
type: docs
weight: 70
url: /sv/java/com.aspose.tasks/datetimeconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class DateTimeConverter extends System.MulticastDelegate
```

Representerar en konverterare för att omvandla datum till sträng i visningsnivåer för tidslinjen.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DateTimeConverter()](#DateTimeConverter--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [invoke(Date date)](#invoke-java.util.Date-) | Representerar en konverteringsmetod för att konvertera datum till sträng i vyens tidslinjenivåer. |
### DateTimeConverter() {#DateTimeConverter--}
```
public DateTimeConverter()
```


### invoke(Date date) {#invoke-java.util.Date-}
```
public abstract String invoke(Date date)
```


Representerar en konverteringsmetod för att konvertera datum till sträng i vyens tidslinjenivåer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| datum | java.util.Date | instansen av klassen `java.util.Date` för att konvertera till sträng. |

**Returns:**
java.lang.String - den strängrepresentation av det angivna datumet.
