---
title: "GlobalizationSettings"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar projektets globaliseringsinställningar."
type: docs
weight: 114
url: /sv/java/com.aspose.tasks/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

Representerar projektets globaliseringsinställningar.

Det rekommenderade sättet är att använda kulturinvarianta litteraler eller format i hela projektet. Men om ett projekt använder kulturspecifika litteraler kan denna klass användas för att hjälpa formelberäkningsmotorn att tolka dessa litteraler.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getFalseLiteral()](#getFalseLiteral--) | Hämtar en sträng för det booleska 'false'-litteralet som används i en formel. |
| [getFormulaDateNA()](#getFormulaDateNA--) | Hämtar "NA" (tomt värde) litteral som används i en formel för ett datumfält. |
| [getTrueLiteral()](#getTrueLiteral--) | Hämtar en sträng för det booleska 'true'-litteralet som används i en formel. |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### getFalseLiteral() {#getFalseLiteral--}
```
public String getFalseLiteral()
```


Hämtar en sträng för det booleska 'false'-litteralet som används i en formel.

**Returns:**
java.lang.String - en sträng för booleskt 'false'-literal som används i en formel.
### getFormulaDateNA() {#getFormulaDateNA--}
```
public String getFormulaDateNA()
```


Hämtar "NA" (tomt värde) litteral som används i en formel för ett datumfält.

**Returns:**
java.lang.String - \"NA\" (tomt värde) literal som används i en formel för ett datumfält.
### getTrueLiteral() {#getTrueLiteral--}
```
public String getTrueLiteral()
```


Hämtar en sträng för det booleska 'true'-litteralet som används i en formel.

**Returns:**
java.lang.String - en sträng för booleskt 'true'-literal som används i en formel.
