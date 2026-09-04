---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu Bildern."
type: docs
weight: 134
url: /de/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu Bildern.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Initialisiert eine neue Instanz der [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions)-Klasse, die zum Speichern gerenderter Bilder im TIFF-, PNG-, BMP- oder JPEG-Format verwendet werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | Gibt die Schriftarteinstellungen an, die beim Rendern der Projektansicht verwendet werden. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Liefert die horizontale Auflösung in dpi. |
| [getJpegQuality()](#getJpegQuality--) | Liefert eine JPEG-Qualität. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Liefert einen benutzerdefinierten Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |
| [getPages()](#getPages--) | Liefert eine Liste von Seitenzahlen, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden sollen. |
| [getPixelFormat()](#getPixelFormat--) | Liefert das Format der Farbdaten für jedes Pixel im Bild. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Liefert einen Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss. |
| [getTiffCompression()](#getTiffCompression--) | Liefert den Kompressionstyp, der beim Speichern generierter Bilder im TIFF-Format angewendet wird. |
| [getVerticalResolution()](#getVerticalResolution--) | Liefert die vertikale Auflösung in dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Legt die horizontale Auflösung in dpi fest. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Legt eine JPEG-Qualität fest. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Legt einen benutzerdefinierten Rückruf fest, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Legt eine Liste von Seitenzahlen fest, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Legt das Format der Farbdaten für jedes Pixel im Bild fest. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Legt einen Wert fest, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Legt den Kompressionstyp fest, der beim Speichern erzeugter Bilder im TIFF-Format angewendet wird. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Legt die vertikale Auflösung in dpi fest. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Initialisiert eine neue Instanz der [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions)-Klasse, die zum Speichern gerenderter Bilder im TIFF-, PNG-, BMP- oder JPEG-Format verwendet werden kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | int | Kann TIFF, PNG, BMP oder JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat) sein. |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Für den internen Gebrauch reserviert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Für den internen Gebrauch reserviert.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Gibt die Schriftarteinstellungen an, die beim Rendern der Projektansicht verwendet werden.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Liefert die horizontale Auflösung in dpi.

**Returns:**
float – die horizontale Auflösung in dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Liest eine JPEG-Qualität. Der zulässige Wertebereich ist 0..100.

**Returns:**
int – eine JPEG-Qualität.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Liefert einen benutzerdefinierten Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Liefert eine Liste von Seitenzahlen, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden sollen.

--------------------

Alle Seiten werden gespeichert, wenn diese Liste leer ist.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; – eine Liste von Seitenzahlen, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Liefert das Format der Farbdaten für jedes Pixel im Bild.

**Returns:**
int – das Format der Farbdaten für jedes Pixel im Bild.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Liefert einen Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss.

**Returns:**
boolean - ein Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Liefert den Kompressionstyp, der beim Speichern generierter Bilder im TIFF-Format angewendet wird.

--------------------

Wirkt nur beim Speichern als TIFF. Der Standardwert ist `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int – der Kompressionstyp, der beim Speichern erzeugter Bilder im TIFF-Format angewendet wird.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Liefert die vertikale Auflösung in dpi.

**Returns:**
float – die vertikale Auflösung in dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Legt die horizontale Auflösung in dpi fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float | die horizontale Auflösung in dpi. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Legt eine JPEG-Qualität fest. Der zulässige Wertebereich ist 0..100.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | eine JPEG-Qualität. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Legt einen benutzerdefinierten Rückruf fest, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | Ein benutzerdefinierter Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Legt eine Liste von Seitenzahlen fest, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden.

--------------------

Alle Seiten werden gespeichert, wenn diese Liste leer ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.List&lt;java.lang.Integer&gt; | eine Liste von Seitenzahlen, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Legt das Format der Farbdaten für jedes Pixel im Bild fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | das Format der Farbdaten für jedes Pixel im Bild. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Legt einen Wert fest, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Legt den Kompressionstyp fest, der beim Speichern erzeugter Bilder im TIFF-Format angewendet wird.

--------------------

Wirkt nur beim Speichern als TIFF. Der Standardwert ist `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Kompressionstyp, der beim Speichern erzeugter Bilder im TIFF-Format angewendet wird. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Legt die vertikale Auflösung in dpi fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float | die vertikale Auflösung in dpi. |

