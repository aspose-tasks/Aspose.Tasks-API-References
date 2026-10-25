---
title: "PdfSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al renderizar páginas del proyecto a PDF."
type: docs
weight: 191
url: /es/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Permite especificar opciones adicionales al renderizar páginas del proyecto a PDF.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Inicializa una nueva instancia de la clase [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) que puede usarse para guardar un documento en el formato [SaveFileFormat](../../com.aspose.tasks/savefileformat). |
## Métodos

| Método | Descripción |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | Obtiene un nivel de cumplimiento deseado para el documento PDF generado. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Obtiene los detalles de cifrado. |
| [getFontSettings()](#getFontSettings--) | Especifica la configuración de fuentes utilizada al renderizar la vista del proyecto. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Obtiene una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [getPages()](#getPages--) | Obtiene la lista de números de página a guardar al guardar el diseño del proyecto en archivos separados. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Obtiene un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Obtiene un valor que indica si se deben guardar las páginas del proyecto en archivos separados. |
| [getTextCompression()](#getTextCompression--) | Obtiene un tipo de compresión que se usará para todos los flujos de contenido, excepto imágenes. |
| [setCompliance(int value)](#setCompliance-int-) | Establece un nivel de cumplimiento deseado para el documento PDF generado. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Establece los detalles de cifrado. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Establece una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Establece la lista de números de página a guardar al guardar el diseño del proyecto en archivos separados. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Establece un valor que indica si se deben guardar las páginas del proyecto en archivos separados. |
| [setTextCompression(int value)](#setTextCompression-int-) | Establece un tipo de compresión que se usará para todos los flujos de contenido, excepto imágenes. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Inicializa una nueva instancia de la clase [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) que puede usarse para guardar un documento en el formato [SaveFileFormat](../../com.aspose.tasks/savefileformat).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
```


Reservado para uso interno.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Reservado para uso interno.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Obtiene un nivel de cumplimiento deseado para el documento PDF generado. El valor predeterminado es [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Returns:**
int - un nivel de cumplimiento deseado para el documento PDF generado.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Obtiene los detalles de cifrado. Si no se establece, no se realizará ningún cifrado.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Especifica la configuración de fuentes utilizada al renderizar la vista del proyecto.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Obtiene una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. Es aplicable cuando se usa la opción `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)).

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Obtiene la lista de números de página a guardar al guardar el diseño del proyecto en archivos separados.

--------------------

Todas las páginas se guardarán si esta lista está vacía.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - la lista de números de página a guardar al guardar el diseño del proyecto en archivos separados.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Obtiene un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

**Returns:**
boolean - un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Obtiene un valor que indica si se deben guardar las páginas del proyecto en archivos separados.

**Returns:**
boolean - un valor que indica si se deben guardar las páginas del proyecto en archivos separados.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Obtiene un tipo de compresión que se usará para todas las secuencias de contenido excepto imágenes. El valor predeterminado es [PdfTextCompression.Flate](../../com.aspose/tasks/pdftextcompression\#Flate).

**Returns:**
int - un tipo de compresión que se usará para todas las secuencias de contenido excepto imágenes.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Establece un nivel de cumplimiento deseado para el documento PDF generado. El valor predeterminado es [PdfCompliance.Pdf15](../../com.aspose/tasks/pdfcompliance\#Pdf15).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un nivel de cumplimiento deseado para el documento PDF generado. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Establece los detalles de cifrado. Si no se establece, no se realizará ningún cifrado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | los detalles de cifrado. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Establece una devolución de llamada definida por el usuario que se usa para obtener un flujo de salida para cada página renderizada. Es aplicable cuando se utiliza la opción `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose/tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose/tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Establece la lista de números de página a guardar al guardar el diseño del proyecto en archivos separados.

--------------------

Todas las páginas se guardarán si esta lista está vacía.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.List&lt;java.lang.Integer&gt; | la lista de números de página que se guardarán al guardar el diseño del proyecto en archivos separados. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Establece un valor que indica si se deben guardar las páginas del proyecto en archivos separados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se deben guardar las páginas del proyecto en archivos separados. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Establece un tipo de compresión que se usará para todas las secuencias de contenido excepto imágenes. El valor predeterminado es [PdfTextCompression.Flate](../../com.aspose/tasks/pdftextcompression\#Flate).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | un tipo de compresión que se usará para todas las secuencias de contenido excepto imágenes. |

