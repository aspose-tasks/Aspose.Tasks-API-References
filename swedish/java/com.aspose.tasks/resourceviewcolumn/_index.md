---
title: "ResourceViewColumn"
second_title: "Aspose.Tasks for Java API-referens"
description: "Projektvy-klass som används i ResourceUsage-vyn och ResourceSheet-vyn."
type: docs
weight: 261
url: /sv/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

Projektets vyklass som används i ResourceUsage-vyn och ResourceSheet-vyn.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Initierar en ny instans av klassen [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Initierar en ny instans av klassen [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Initierar en ny instans av klassen [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Konverterar aktuell resurs till kolumntexten. |
| [getField()](#getField--) | Returnerar kolumnfältet. |
| [setField(int value)](#setField-int-) | Ställer in kolumnfältet. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Initierar en ny instans av klassen [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Kolumnens namn. |
| width | int | Kolumnens bredd i pixlar. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Resursdata till kolumntextkonverterare. |
| fält | int | Kolumnfält. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Initierar en ny instans av klassen [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Kolumnens namn. |
| width | int | Kolumnens bredd i pixlar. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Resursdata till kolumntextkonverterare. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Initierar en ny instans av klassen [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| width | int | Kolumnbredd i pixlar. |
| fält | int | Kolumnfält. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Konverterar aktuell resurs till kolumntexten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Aktuell resurs. |

**Returns:**
java.lang.String - Kolumntexten.
### getField() {#getField--}
```
public int getField()
```


Returnerar kolumnfältet. `Field`.

**Returns:**
int - kolumnfältets värde.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Ställer in kolumnfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | kolumnfältets värde. |

