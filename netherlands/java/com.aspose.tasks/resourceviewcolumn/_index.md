---
title: "ResourceViewColumn"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Projectenweergaveklasse die wordt gebruikt in de ResourceUsage-weergave en de ResourceSheet-weergave."
type: docs
weight: 261
url: /nl/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

Projectweergaveklasse die wordt gebruikt in de ResourceUsage-weergave en de ResourceSheet-weergave.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Initialiseert een nieuw exemplaar van de [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) klasse. |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Initialiseert een nieuw exemplaar van de [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) klasse. |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Initialiseert een nieuw exemplaar van de [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Converteert de huidige resource naar de kolomtekst. |
| [getField()](#getField--) | Retourneert kolomveld. |
| [setField(int value)](#setField-int-) | Stelt kolomveld in. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Initialiseert een nieuw exemplaar van de [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | Naam van de kolom. |
| breedte | int | Breedte van de kolom in pixels. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Resource-gegevens naar kolomtekst converter. |
| veld | int | Kolomveld. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Initialiseert een nieuw exemplaar van de [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | Naam van de kolom. |
| breedte | int | Breedte van de kolom in pixels. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Resource-gegevens naar kolomtekst converter. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Initialiseert een nieuw exemplaar van de [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| breedte | int | Kolombreedte in pixels. |
| veld | int | Kolomveld. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Converteert de huidige resource naar de kolomtekst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Huidige resource. |

**Returns:**
java.lang.String - De kolomtekst.
### getField() {#getField--}
```
public int getField()
```


Retourneert kolomveld. `Field`.

**Returns:**
int - kolomveldwaarde.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Stelt kolomveld in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | kolomveldwaarde. |

