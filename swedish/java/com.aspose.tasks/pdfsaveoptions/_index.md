---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Tillåter att ange ytterligare alternativ vid rendering av projektsidor till PDF."
type: docs
weight: 191
url: /sv/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Tillåter att ange ytterligare alternativ vid rendering av projektsidor till PDF.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initierar en ny instans av klassen [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) som kan användas för att spara ett dokument i formatet [SaveFileFormat](../../com.aspose.tasks/savefileformat). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | Hämtar önskad efterlevnadsnivå för genererat PDF-dokument. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Hämtar krypteringsdetaljer. |
| [getFontSettings()](#getFontSettings--) | Anger teckensnittsinställningar som används när projektets vy renderas. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Hämtar en användardefinierad återuppringning som används för att få en utström för varje renderad sida. |
| [getPages()](#getPages--) | Hämtar listan med sidnummer som ska sparas när projektlayouten sparas till separata filer. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Hämtar ett värde som indikerar om ett gap mellan sista uppgiften och sidfoten ska minskas. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Hämtar ett värde som indikerar om projektets sidor ska sparas till separata filer. |
| [getTextCompression()](#getTextCompression--) | Hämtar en komprimeringstyp som ska användas för alla innehållsströmmar förutom bilder. |
| [setCompliance(int value)](#setCompliance-int-) | Ställer in önskad efterlevnadsnivå för genererat PDF-dokument. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Ställer in krypteringsdetaljer. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Ställer in ett användardefinierat återanrop som används för att hämta en utdataström för varje renderad sida. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Ställer in listan med sidnummer som ska sparas när projektlayouten sparas till separata filer. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Ställer in ett värde som anger om ett mellanrum mellan sista uppgiften och sidfoten ska minskas. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Ställer in ett värde som anger om projektsidor ska sparas i separata filer. |
| [setTextCompression(int value)](#setTextCompression-int-) | Ställer in en komprimeringstyp som ska användas för alla innehållsströmmar förutom bilder. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initierar en ny instans av klassen [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) som kan användas för att spara ett dokument i formatet [SaveFileFormat](../../com.aspose.tasks/savefileformat).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
```


Reserverad för intern användning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Reserverad för intern användning.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Hämtar önskad efterlevnadsnivå för genererat PDF‑dokument. Standard är [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Returns:**
int – en önskad efterlevnadsnivå för genererat PDF‑dokument.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Hämtar krypteringsdetaljer. Om den inte är angiven utförs ingen kryptering.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Anger teckensnittsinställningar som används när projektets vy renderas.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Hämtar en användardefinierad återuppringning som används för att få en utdataström för varje renderad sida. Gäller när alternativet `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) används.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Hämtar listan med sidnummer som ska sparas när projektlayouten sparas till separata filer.

--------------------

Alla sidor sparas om den här listan är tom.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; – listan med sidnummer som ska sparas när projektdesign sparas i separata filer.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Hämtar ett värde som indikerar om ett gap mellan sista uppgiften och sidfoten ska minskas.

**Returns:**
boolean - ett värde som anger om ett mellanrum mellan sista uppgiften och sidfoten ska minskas.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Hämtar ett värde som indikerar om projektets sidor ska sparas till separata filer.

**Returns:**
boolean – ett värde som anger om projektsidor ska sparas i separata filer.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Hämtar en komprimeringstyp som ska användas för alla innehållsströmmar förutom bilder. Standard är [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Returns:**
int – en komprimeringstyp som ska användas för alla innehållsströmmar förutom bilder.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Ställer in en önskad efterlevnadsnivå för genererat PDF‑dokument. Standard är [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en önskad efterlevnadsnivå för genererat PDF‑dokument. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Ställer in krypteringsdetaljer. Om den inte är angiven utförs ingen kryptering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | en krypteringsdetalj. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Ställer in en användardefinierad återuppringning som används för att få en utdataström för varje renderad sida. Gäller när alternativet `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) används.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | ett användardefinierat återanrop som används för att hämta en utström för varje renderad sida. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Ställer in listan med sidnummer som ska sparas när projektlayouten sparas till separata filer.

--------------------

Alla sidor sparas om den här listan är tom.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.List&lt;java.lang.Integer&gt; | listan med sidnummer som ska sparas när projektdesign sparas i separata filer. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Ställer in ett värde som anger om ett mellanrum mellan sista uppgiften och sidfoten ska minskas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om ett mellanrum mellan sista uppgift och sidfot ska minskas. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Ställer in ett värde som anger om projektsidor ska sparas i separata filer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som anger om projektsidor ska sparas i separata filer. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Ställer in en komprimeringstyp som ska användas för alla innehållsströmmar förutom bilder. Standard är [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | en komprimeringstyp som ska användas för alla innehållsströmmar förutom bilder. |

