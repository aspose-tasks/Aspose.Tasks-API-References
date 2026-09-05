---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Staat toe om extra opties op te geven bij het renderen van projectpagina's naar PDF."
type: docs
weight: 191
url: /nl/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Staat toe om extra opties op te geven bij het renderen van projectpagina's naar PDF.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initialiseert een nieuw exemplaar van de [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) klasse die kan worden gebruikt om een document op te slaan in het [SaveFileFormat](../../com.aspose.tasks/savefileformat) formaat. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | Haalt een gewenst nalevingsniveau op voor het gegenereerde PDF-document. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Haalt encryptiedetails op. |
| [getFontSettings()](#getFontSettings--) | Specificeert lettertype‑instellingen die worden gebruikt bij het renderen van de projectweergave. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Haalt een door de gebruiker gedefinieerde callback op die wordt gebruikt om een uitvoerstroom voor elke gerenderde pagina te verkrijgen. |
| [getPages()](#getPages--) | Haalt de lijst met paginanummers op die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Haalt een waarde op die aangeeft of een kloof tussen de laatste taak en de voettekst moet worden verkleind. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Haalt een waarde op die aangeeft of projectpagina's naar afzonderlijke bestanden moeten worden opgeslagen. |
| [getTextCompression()](#getTextCompression--) | Haalt een compressietype op dat moet worden gebruikt voor alle contentstreams behalve afbeeldingen. |
| [setCompliance(int value)](#setCompliance-int-) | Stelt een gewenst nalevingsniveau in voor het gegenereerde PDF-document. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Stelt encryptiedetails in. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Stelt een door de gebruiker gedefinieerde callback in die wordt gebruikt om een output‑stream voor elke gerenderde pagina te verkrijgen. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Stelt de lijst met paginanummers in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Stelt een waarde in die aangeeft of projectpagina's naar afzonderlijke bestanden moeten worden opgeslagen. |
| [setTextCompression(int value)](#setTextCompression-int-) | Stelt een compressietype in dat moet worden gebruikt voor alle contentstreams behalve afbeeldingen. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initialiseert een nieuw exemplaar van de [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) klasse die kan worden gebruikt om een document op te slaan in het [SaveFileFormat](../../com.aspose.tasks/savefileformat) formaat.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
```


Gereserveerd voor intern gebruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Gereserveerd voor intern gebruik.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Haalt een gewenst nalevingsniveau op voor het gegenereerde PDF-document. Standaard is [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Returns:**
int - een gewenst nalevingsniveau voor het gegenereerde PDF-document.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Haalt encryptiedetails op. Indien niet ingesteld, wordt er geen encryptie uitgevoerd.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Specificeert lettertype‑instellingen die worden gebruikt bij het renderen van de projectweergave.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Haalt een door de gebruiker gedefinieerde callback op die wordt gebruikt om een outputstream te verkrijgen voor elke gerenderde pagina. Is van toepassing wanneer de optie `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) wordt gebruikt.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Haalt de lijst met paginanummers op die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden.

--------------------

Alle pagina's worden opgeslagen als deze lijst leeg is.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - de lijst met paginanummers die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Haalt een waarde op die aangeeft of een kloof tussen de laatste taak en de voettekst moet worden verkleind.

**Returns:**
boolean - een waarde die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Haalt een waarde op die aangeeft of projectpagina's naar afzonderlijke bestanden moeten worden opgeslagen.

**Returns:**
boolean - een waarde die aangeeft of projectpagina's naar afzonderlijke bestanden moeten worden opgeslagen.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Haalt een compressietype op dat wordt gebruikt voor alle inhoudsstromen behalve afbeeldingen. Standaard is [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Returns:**
int - een compressietype dat wordt gebruikt voor alle inhoudsstromen behalve afbeeldingen.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Stelt een gewenst conformiteitsniveau in voor het gegenereerde PDF-document. Standaard is [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een gewenst conformiteitsniveau voor het gegenereerde PDF-document. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Stelt encryptiedetails in. Als dit niet is ingesteld, wordt er geen encryptie uitgevoerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | een encryptiedetail. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Stelt een door de gebruiker gedefinieerde callback in die wordt gebruikt om een uitvoerstroom te verkrijgen voor elke gerenderde pagina. Is van toepassing wanneer de optie `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) wordt gebruikt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | een door de gebruiker gedefinieerde callback die wordt gebruikt om een output-stream voor elke gerenderde pagina te verkrijgen. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Stelt de lijst met paginanummers in die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden.

--------------------

Alle pagina's worden opgeslagen als deze lijst leeg is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.List&lt;java.lang.Integer&gt; | de lijst met paginanummers die moeten worden opgeslagen bij het opslaan van de projectlay-out naar afzonderlijke bestanden. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Stelt een waarde in die aangeeft of de ruimte tussen de laatste taak en de voettekst moet worden verkleind.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of een ruimte tussen de laatste taak en de voettekst moet worden verkleind. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Stelt een waarde in die aangeeft of projectpagina's naar afzonderlijke bestanden moeten worden opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of projectpagina's naar afzonderlijke bestanden moeten worden opgeslagen. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Stelt een compressietype in dat wordt gebruikt voor alle inhoudsstromen behalve afbeeldingen. Standaard is [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een compressietype dat wordt gebruikt voor alle inhoudsstromen behalve afbeeldingen. |

