---
title: "ResourceViewColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "Projektansichts‑Klasse, die in der ResourceUsage‑Ansicht und der ResourceSheet‑Ansicht verwendet wird."
type: docs
weight: 261
url: /de/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

Projektansichtsklasse, die in der ResourceUsage-Ansicht und der ResourceSheet-Ansicht verwendet wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Initialisiert eine neue Instanz der [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)-Klasse. |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Initialisiert eine neue Instanz der [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)-Klasse. |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Initialisiert eine neue Instanz der [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Konvertiert die aktuelle Ressource in den Spaltentext. |
| [getField()](#getField--) | Gibt das Spaltenfeld zurück. |
| [setField(int value)](#setField-int-) | Setzt das Spaltenfeld. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Initialisiert eine neue Instanz der [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Name der Spalte. |
| width | int | Breite der Spalte in Pixeln. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Ressourcendaten‑zu‑Spaltentext‑Konverter. |
| field | int | Spaltenfeld. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Initialisiert eine neue Instanz der [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Name der Spalte. |
| width | int | Breite der Spalte in Pixeln. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Ressourcendaten‑zu‑Spaltentext‑Konverter. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Initialisiert eine neue Instanz der [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| width | int | Spaltenbreite in Pixeln. |
| field | int | Spaltenfeld. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Konvertiert die aktuelle Ressource in den Spaltentext.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Aktuelle Ressource. |

**Returns:**
java.lang.String - Der Spaltentext.
### getField() {#getField--}
```
public int getField()
```


Gibt das Spaltenfeld zurück. `Field`.

**Returns:**
int - Wert des Spaltenfelds.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Setzt das Spaltenfeld.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Wert des Spaltenfelds. |

