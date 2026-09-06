---
title: "ImageSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al renderizar páginas del proyecto a imágenes."
type: docs
weight: 134
url: /es/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Permite especificar opciones adicionales al renderizar páginas del proyecto a imágenes.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Inicializa una nueva instancia de la clase [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) que puede usarse para guardar imágenes renderizadas en formatos TIFF, PNG, BMP o JPEG. |
## Métodos

| Método | Descripción |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | Especifica la configuración de fuentes utilizada al renderizar la vista del proyecto. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Obtiene la resolución horizontal en dpi. |
| [getJpegQuality()](#getJpegQuality--) | Obtiene la calidad JPEG. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Obtiene una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [getPages()](#getPages--) | Obtiene una lista de números de página para guardar al guardar el diseño del proyecto en archivos separados. |
| [getPixelFormat()](#getPixelFormat--) | Obtiene el formato de los datos de color para cada píxel en la imagen. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Obtiene un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |
| [getTiffCompression()](#getTiffCompression--) | Obtiene el tipo de compresión a aplicar al guardar imágenes generadas en formato TIFF. |
| [getVerticalResolution()](#getVerticalResolution--) | Obtiene la resolución vertical en dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Establece la resolución horizontal en dpi. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Establece una calidad JPEG. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Establece una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Establece una lista de números de página para guardar al guardar el diseño del proyecto en archivos separados. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Establece el formato de los datos de color para cada píxel en la imagen. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Establece el tipo de compresión a aplicar al guardar imágenes generadas en formato TIFF. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Establece la resolución vertical en dpi. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Inicializa una nueva instancia de la clase [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) que puede usarse para guardar imágenes renderizadas en formatos TIFF, PNG, BMP o JPEG.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | int | Puede ser TIFF, PNG, BMP o JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat). |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
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
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Especifica la configuración de fuentes utilizada al renderizar la vista del proyecto.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Obtiene la resolución horizontal en dpi.

**Returns:**
float - la resolución horizontal en dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Obtiene una calidad JPEG. El rango de valores permitido es 0..100.

**Returns:**
int - una calidad JPEG.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Obtiene una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Obtiene una lista de números de página para guardar al guardar el diseño del proyecto en archivos separados.

--------------------

Todas las páginas se guardarán si esta lista está vacía.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - una lista de números de página para guardar al guardar el diseño del proyecto en archivos separados.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Obtiene el formato de los datos de color para cada píxel en la imagen.

**Returns:**
int - el formato de los datos de color para cada píxel en la imagen.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Obtiene un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

**Returns:**
boolean - un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Obtiene el tipo de compresión a aplicar al guardar imágenes generadas en formato TIFF.

--------------------

Solo tiene efecto al guardar en TIFF. El valor predeterminado es `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - el tipo de compresión a aplicar al guardar imágenes generadas en formato TIFF.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Obtiene la resolución vertical en dpi.

**Returns:**
float - la resolución vertical en dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Establece la resolución horizontal en dpi.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float | la resolución horizontal en ppp. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Establece una calidad JPEG. El rango de valores permitido es 0..100.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | una calidad JPEG. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Establece una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Establece una lista de números de página para guardar al guardar el diseño del proyecto en archivos separados.

--------------------

Todas las páginas se guardarán si esta lista está vacía.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.List&lt;java.lang.Integer&gt; | una lista de números de página para guardar al guardar el diseño del proyecto en archivos separados. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Establece el formato de los datos de color para cada píxel en la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el formato de los datos de color para cada píxel en la imagen. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Establece el tipo de compresión a aplicar al guardar imágenes generadas en formato TIFF.

--------------------

Solo tiene efecto al guardar en TIFF. El valor predeterminado es `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el tipo de compresión a aplicar al guardar imágenes generadas en formato TIFF. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Establece la resolución vertical en dpi.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float | la resolución vertical en ppp. |

