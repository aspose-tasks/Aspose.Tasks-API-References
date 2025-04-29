---
title: PdfSaveOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when rendering project pages to PDF.
type: docs
weight: 190
url: /java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Allows to specify additional options when rendering project pages to PDF.
## Constructors

| Constructor | Description |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initializes a new instance of the [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) class that can be used to save a document in the [SaveFileFormat](../../com.aspose.tasks/savefileformat) format. |
## Methods

| Method | Description |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | Gets a desired compliance level for generated PDF document. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Gets an encryption details. |
| [getFontSettings()](#getFontSettings--) | Specifies font settings used when rendering project's view. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Gets a user-defined callback which is used to get an output stream for each rendered page. |
| [getPages()](#getPages--) | Gets the list of pages numbers to save when saving project layout to separate files. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Gets a value indicating whether a gap between last task and the footer must be reduced. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Gets a value indicating whether to save project pages to separate files. |
| [getTextCompression()](#getTextCompression--) | Gets a compression type to be used for all content streams except images. |
| [setCompliance(int value)](#setCompliance-int-) | Sets a desired compliance level for generated PDF document. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Sets a encryption details. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Sets a user-defined callback which is used to get an output stream for each rendered page. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Sets the list of pages numbers to save when saving project layout to separate files. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Sets a value indicating whether a gap between last task and the footer must be reduced. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Sets a value indicating whether to save project pages to separate files. |
| [setTextCompression(int value)](#setTextCompression-int-) | Sets a compression type to be used for all content streams except images. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initializes a new instance of the [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) class that can be used to save a document in the [SaveFileFormat](../../com.aspose.tasks/savefileformat) format.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
```


Reserved for internal usage.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Reserved for internal usage.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Gets a desired compliance level for generated PDF document. Default is [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Returns:**
int - a desired compliance level for generated PDF document.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Gets an encryption details. If not set, then no encryption will be performed.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Specifies font settings used when rendering project's view.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Gets a user-defined callback which is used to get an output stream for each rendered page. Is applicable when `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) option is used.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Gets the list of pages numbers to save when saving project layout to separate files.

--------------------

All pages will be saved if this list is empty.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - the list of pages numbers to save when saving project layout to separate files.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Gets a value indicating whether a gap between last task and the footer must be reduced.

**Returns:**
boolean - a value indicating whether a gap between last task and the footer must be reduced.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Gets a value indicating whether to save project pages to separate files.

**Returns:**
boolean - a value indicating whether to save project pages to separate files.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Gets a compression type to be used for all content streams except images. Default is [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Returns:**
int - a compression type to be used for all content streams except images.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Sets a desired compliance level for generated PDF document. Default is [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a desired compliance level for generated PDF document. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Sets a encryption details. If not set, then no encryption will be performed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | a encryption details. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Sets a user-defined callback which is used to get an output stream for each rendered page. Is applicable when `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) option is used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | a user-defined callback which is used to get an output stream for each rendered page. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Sets the list of pages numbers to save when saving project layout to separate files.

--------------------

All pages will be saved if this list is empty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;java.lang.Integer&gt; | the list of pages numbers to save when saving project layout to separate files. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Sets a value indicating whether a gap between last task and the footer must be reduced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether a gap between last task and the footer must be reduced. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Sets a value indicating whether to save project pages to separate files.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to save project pages to separate files. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Sets a compression type to be used for all content streams except images. Default is [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a compression type to be used for all content streams except images. |

