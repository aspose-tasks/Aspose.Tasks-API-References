---
title: "TableTextStyle"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een tekststijl in een weergavetabel voor."
type: docs
weight: 288
url: /nl/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

Stelt een tekststijl in een weergavetabel voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | Initialiseert een nieuw exemplaar van de [TableTextStyle](../../com.aspose.tasks/tabletextstyle) klasse. |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | Initialiseert een nieuw exemplaar van de [TableTextStyle](../../com.aspose.tasks/tabletextstyle) klasse met het opgegeven lettertype. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | Initialiseert een nieuw exemplaar van de [TableTextStyle](../../com.aspose.tasks/tabletextstyle) klasse met de opgegeven lettergrootte en lettertype‑stijl. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | Initialiseert een nieuw exemplaar van de [TableTextStyle](../../com.aspose.tasks/tabletextstyle) klasse met de standaard lettertype‑instellingen en de opgegeven lettertype‑stijl. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getField()](#getField--) | Haalt een veld op waarop de stijl moet worden toegepast. |
| [getItemType()](#getItemType--) | Retourneert het type tekstitem. |
| [getRowUid()](#getRowUid--) | Haalt een unieke rij‑ID op. |
| [setField(int value)](#setField-int-) | Stelt een veld in waarop de stijl moet worden toegepast. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


Initialiseert een nieuw exemplaar van de [TableTextStyle](../../com.aspose.tasks/tabletextstyle) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowUid | int | Een opgegeven unieke rij‑ID. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


Initialiseert een nieuw exemplaar van de [TableTextStyle](../../com.aspose.tasks/tabletextstyle) klasse met het opgegeven lettertype.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowUid | int | Een opgegeven unieke rij‑ID. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Een lettertype waarop een tekststijl is gebaseerd. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


Initialiseert een nieuw exemplaar van de [TableTextStyle](../../com.aspose.tasks/tabletextstyle) klasse met de opgegeven lettergrootte en lettertype‑stijl.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowUid | int | Een opgegeven unieke rij‑ID. |
| fontSize | float | Grootte van een lettertype waarop een tekststijl is gebaseerd. |
| fontStyle | int | Lettertype stijl. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


Initialiseert een nieuw exemplaar van de [TableTextStyle](../../com.aspose.tasks/tabletextstyle) klasse met de standaard lettertype‑instellingen en de opgegeven lettertype‑stijl.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| rowUid | int | Een opgegeven unieke rij‑ID. |
| fontStyle | int | Lettertype stijl. |

### getField() {#getField--}
```
public final int getField()
```


Haalt een veld op waarop de stijl moet worden toegepast. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - een veld waarop de stijl moet worden toegepast.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Retourneert het type tekstitem.

**Returns:**
int - TextItemType genummerde typewaarde.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


Haalt een unieke rij‑ID op.

--------------------

Geef -1 terug als de stijl moet worden toegepast op alle rijen van een weergave.

**Returns:**
int - een unieke rij-id.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Stelt een veld in waarop de stijl moet worden toegepast. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een veld waarop de stijl moet worden toegepast. |

