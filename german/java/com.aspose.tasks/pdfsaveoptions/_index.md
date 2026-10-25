---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu PDF."
type: docs
weight: 191
url: /de/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Projektseiten zu PDF.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initialisiert eine neue Instanz der Klasse [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions), die verwendet werden kann, um ein Dokument im Format [SaveFileFormat](../../com.aspose.tasks/savefileformat) zu speichern. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | Gibt einen gewünschten Konformitätsgrad für das erzeugte PDF‑Dokument zurück. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Gibt Verschlüsselungsdetails zurück. |
| [getFontSettings()](#getFontSettings--) | Gibt die Schriftarteinstellungen an, die beim Rendern der Projektansicht verwendet werden. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Liefert einen benutzerdefinierten Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |
| [getPages()](#getPages--) | Liefert die Liste der Seitennummern, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Liefert einen Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Liefert einen Wert, der angibt, ob Projektseiten in separate Dateien gespeichert werden sollen. |
| [getTextCompression()](#getTextCompression--) | Liefert einen Kompressionstyp, der für alle Inhaltsströme außer Bildern verwendet wird. |
| [setCompliance(int value)](#setCompliance-int-) | Legt ein gewünschtes Konformitätsniveau für das erzeugte PDF-Dokument fest. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Legt Verschlüsselungsdetails fest. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Legt einen benutzerdefinierten Rückruf fest, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Legt die Liste der Seitennummern fest, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Legt einen Wert fest, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Legt einen Wert fest, der angibt, ob Projektseiten in separate Dateien gespeichert werden sollen. |
| [setTextCompression(int value)](#setTextCompression-int-) | Legt einen Kompressionstyp fest, der für alle Inhaltsströme außer Bildern verwendet wird. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initialisiert eine neue Instanz der Klasse [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions), die verwendet werden kann, um ein Dokument im Format [SaveFileFormat](../../com.aspose.tasks/savefileformat) zu speichern.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
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
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Liefert ein gewünschtes Konformitätsniveau für das erzeugte PDF-Dokument. Standard ist [PdfCompliance.Pdf15](../../com.aspose/tasks/pdfcompliance\#Pdf15).

**Returns:**
int – ein gewünschtes Konformitätsniveau für das erzeugte PDF-Dokument.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Liefert Verschlüsselungsdetails. Wenn nicht festgelegt, wird keine Verschlüsselung durchgeführt.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Gibt die Schriftarteinstellungen an, die beim Rendern der Projektansicht verwendet werden.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Liefert einen benutzerdefinierten Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. Gilt, wenn die Option `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose/tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose/tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) verwendet wird.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Liefert die Liste der Seitennummern, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden.

--------------------

Alle Seiten werden gespeichert, wenn diese Liste leer ist.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; – die Liste der Seitennummern, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Liefert einen Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss.

**Returns:**
boolean - ein Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Liefert einen Wert, der angibt, ob Projektseiten in separate Dateien gespeichert werden sollen.

**Returns:**
boolean – ein Wert, der angibt, ob Projektseiten in separate Dateien gespeichert werden sollen.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Liefert einen Kompressionstyp, der für alle Inhaltsströme außer Bildern verwendet wird. Standard ist [PdfTextCompression.Flate](../../com.aspose/tasks/pdftextcompression\#Flate).

**Returns:**
int – ein Kompressionstyp, der für alle Inhaltsströme außer Bildern verwendet wird.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Legt ein gewünschtes Konformitätsniveau für das erzeugte PDF-Dokument fest. Standard ist [PdfCompliance.Pdf15](../../com.aspose/tasks/pdfcompliance\#Pdf15).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein gewünschtes Konformitätsniveau für das erzeugte PDF-Dokument. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Legt Verschlüsselungsdetails fest. Wenn nicht festgelegt, wird keine Verschlüsselung durchgeführt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | Verschlüsselungsdetails. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Legt einen benutzerdefinierten Callback fest, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. Gilt, wenn die Option `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose/tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose/tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | Ein benutzerdefinierter Callback, der verwendet wird, um einen Ausgabestream für jede gerenderte Seite zu erhalten. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Legt die Liste der Seitennummern fest, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden.

--------------------

Alle Seiten werden gespeichert, wenn diese Liste leer ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.List&lt;java.lang.Integer&gt; | die Liste der Seitennummern, die beim Speichern des Projektlayouts in separate Dateien gespeichert werden. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Legt einen Wert fest, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob ein Abstand zwischen der letzten Aufgabe und der Fußzeile reduziert werden muss. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Legt einen Wert fest, der angibt, ob Projektseiten in separate Dateien gespeichert werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Projektseiten in separate Dateien gespeichert werden sollen. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Legt einen Kompressionstyp fest, der für alle Inhaltsströme außer Bildern verwendet wird. Standard ist [PdfTextCompression.Flate](../../com.aspose/tasks/pdftextcompression\#Flate).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Ein Kompressionstyp, der für alle Inhaltsströme außer Bildern verwendet wird. |

