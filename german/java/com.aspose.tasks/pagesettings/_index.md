---
title: "PageSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt Druckeinstellungen für eine Seite der Projektansicht dar."
type: docs
weight: 181
url: /de/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

Stellt Druckeinstellungen für eine Seite der Projektansicht dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PageSettings()](#PageSettings--) | Initialisiert eine neue Instanz der [PageSettings](../../com.aspose/tasks/pagesettings)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | Gibt einen Wert zurück, der angibt, ob der Druck auf den angegebenen Prozentsatz (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) der Normalgröße angepasst werden soll. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Gibt die erste Seitennummer für den Druck zurück. |
| [getPagesInHeight()](#getPagesInHeight--) | Gibt die Anzahl der zu druckenden Seiten in der Höhe zurück. |
| [getPagesInWidth()](#getPagesInWidth--) | Gibt die Anzahl der zu druckenden Seiten in der Breite zurück. |
| [getPaperSize()](#getPaperSize--) | Gibt die Papiergröße zurück. |
| [getPaperSizeId()](#getPaperSizeId--) | Gibt einen Integer zurück, der einen der Werte von PrinterPaperSize oder eine benutzerdefinierte Seitengrößen-ID darstellt. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | Gibt den Prozentsatz der Normalgröße zurück, auf den der Druck angepasst werden soll. |
| [isPortrait()](#isPortrait--) | Gibt einen Wert zurück, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | Setzt einen Wert, der angibt, ob der Druck auf den angegebenen Prozentsatz (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) der Normalgröße angepasst werden soll. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | Setzt die erste Seitennummer für den Druck. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | Setzt die Anzahl der zu druckenden Seiten in der Höhe. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | Setzt die Anzahl der zu druckenden Seiten in der Breite. |
| [setPaperSize(int value)](#setPaperSize-int-) | Setzt die Papiergröße. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | Setzt einen Integer, der einen der Werte von PrinterPaperSize oder eine benutzerdefinierte Seitengrößen-ID darstellt. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | Setzt den Prozentsatz der Normalgröße, auf den der Druck angepasst werden soll. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Setzt einen Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


Initialisiert eine neue Instanz der [PageSettings](../../com.aspose/tasks/pagesettings)-Klasse. Stellt die Druckeinstellungen für eine Seite der Projektansicht dar.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


Gibt einen Wert zurück, der angibt, ob der Druck auf den angegebenen Prozentsatz (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) der Normalgröße angepasst werden soll.

--------------------

Wirkt nicht, wenn das Projekt im HTML-Format gerendert wird.

**Returns:**
boolean – ein Wert, der angibt, ob der Druck auf den angegebenen Prozentsatz (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) der Normalgröße angepasst werden soll.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


Gibt die erste Seitennummer für den Druck zurück.

**Returns:**
short – die erste Seitennummer für den Druck.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


Gibt die Anzahl der zu druckenden Seiten in der Höhe zurück.

**Returns:**
int – die Anzahl der zu druckenden Seiten in der Höhe.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


Gibt die Anzahl der zu druckenden Seiten in der Breite zurück.

**Returns:**
int – die Anzahl der zu druckenden Seiten in der Breite.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


Gibt die Papiergröße zurück. Kann einer der Werte der [PrinterPaperSize](../../com.aspose/tasks/printerpapersize)-Aufzählung sein.

**Returns:**
int - ein Papierformat.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


Ermittelt einen Integer, der einen der PrinterPaperSize-Werte oder eine benutzerdefinierte Seitengrößen-ID darstellt. Dieser Wert kann verwendet werden, um PaperSize aus den OS-Einstellungen () zu erhalten.

**Returns:**
int - ein Integer, der einen der PrinterPaperSize-Werte oder eine benutzerdefinierte Seitengrößen-ID darstellt.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


Gibt den Prozentsatz der Normalgröße zurück, auf den der Druck angepasst werden soll.

**Returns:**
int - ein Prozentsatz der Normalgröße, auf den der Druck angepasst werden soll.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Gibt einen Wert zurück, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist.

--------------------

Ist während des Renderns anwendbar, wenn SaveOptions.getPageSize() == PageSize.DefinedInView.

**Returns:**
boolean - ein Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


Setzt einen Wert, der angibt, ob der Druck auf den angegebenen Prozentsatz (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) der Normalgröße angepasst werden soll.

--------------------

Wirkt nicht, wenn das Projekt im HTML-Format gerendert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | boolean | ein Wert, der angibt, ob der Druck auf den angegebenen Prozentsatz (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) der Normalgröße angepasst werden soll. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


Setzt die erste Seitennummer für den Druck.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short | eine erste Seitennummer für den Druck. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


Setzt die Anzahl der zu druckenden Seiten in der Höhe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Seiten in der Höhe, die gedruckt werden sollen. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


Setzt die Anzahl der zu druckenden Seiten in der Breite.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine Anzahl von Seiten in der Breite, die gedruckt werden sollen. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


Legt ein Papierformat fest. Kann einer der Werte der Aufzählung [PrinterPaperSize](../../com.aspose.tasks/printerpapersize) sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Papierformat. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


Legt einen Integer fest, der einen der PrinterPaperSize-Werte oder eine benutzerdefinierte Seitengrößen-ID darstellt. Dieser Wert kann verwendet werden, um PaperSize aus den OS-Einstellungen () zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Integer, der einen der PrinterPaperSize-Werte oder eine benutzerdefinierte Seitengrößen-ID darstellt. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


Setzt den Prozentsatz der Normalgröße, auf den der Druck angepasst werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Prozentsatz der Normalgröße, auf den der Druck angepasst werden soll. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Setzt einen Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist.

--------------------

Ist während des Renderns anwendbar, wenn SaveOptions.getPageSize() == PageSize.DefinedInView.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist. |

