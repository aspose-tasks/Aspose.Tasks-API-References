---
title: "CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling av anpassade projektegenskaper."
type: docs
weight: 61
url: /sv/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Representerar en samling av anpassade projektegenskaper.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Initierar en ny instans av klassen [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Skapar en ny anpassad egenskap. |
| [add(String name, double value)](#add-java.lang.String-double-) | Skapar en ny anpassad egenskap. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Skapar en ny anpassad egenskap. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Skapar en ny anpassad egenskap. |
| [clear()](#clear--) | Rensar PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | Hämtar ett värde som anger om den här samlingen är skrivskyddad; annars falskt. |
| [remove(String name)](#remove-java.lang.String-) | Tar bort en egenskap med det angivna namnet från samlingen. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Initierar en ny instans av klassen [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection).

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Skapar en ny anpassad egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| värde | boolean | Värdet för det nyss skapade egenskapsobjektet. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Skapar en ny anpassad egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| värde | double | Värdet för det nyss skapade egenskapsobjektet. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Skapar en ny anpassad egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| värde | java.lang.String | Värdet för det nyss skapade egenskapsobjektet. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Skapar en ny anpassad egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på egenskapen. |
| värde | java.util.Date | Värdet för det nyss skapade egenskapsobjektet. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


Rensar PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Hämtar ett värde som anger om den här samlingen är skrivskyddad; annars falskt.

**Returns:**
boolean - ett värde som indikerar om denna samling är skrivskyddad; annars falskt.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Tar bort en egenskap med det angivna namnet från samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Det skiftlägesokänsliga namnet på egenskapen. |

**Returns:**
boolean - True om elementet hittas och tas bort; annars false.
