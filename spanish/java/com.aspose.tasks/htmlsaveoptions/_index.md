---
title: "HtmlSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al renderizar páginas del proyecto a HTML."
type: docs
weight: 132
url: /es/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Permite especificar opciones adicionales al renderizar páginas del proyecto a HTML.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Inicializa una nueva instancia de la clase [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | Obtiene la devolución de llamada que se llama para crear el recurso que almacena CSS. |
| [getCssStylePrefix()](#getCssStylePrefix--) | Obtiene el prefijo de estilo CSS. |
| [getExportCss()](#getExportCss--) | Obtiene la forma en que se exporta CSS. |
| [getExportFonts()](#getExportFonts--) | Obtiene la forma en que se exportan las fuentes. |
| [getExportImages()](#getExportImages--) | Obtiene la forma en que se exportan las imágenes. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Obtiene los tipos de fuentes. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Obtiene la devolución de llamada que se llama para crear el recurso que almacena la fuente. |
| [getFontSettings()](#getFontSettings--) | Especifica la configuración de fuentes utilizada al renderizar la vista del proyecto. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Obtiene la devolución de llamada que se llama para crear el recurso que almacena la fuente. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Obtiene un valor que indica si se debe incluir el nombre del proyecto en el encabezado de la página HTML. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Obtiene un valor que indica si se debe incluir el nombre del proyecto en el título HTML. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Obtiene una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [getPages()](#getPages--) | Obtiene una lista de números de página para guardar al renderizar el diseño del proyecto. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Obtiene un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Obtiene un valor que indica si se debe usar un pincel degradado al renderizar el diseño del proyecto. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | Establece la devolución de llamada que se llama para crear el recurso que almacena CSS. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | Establece el prefijo de estilo CSS. |
| [setExportCss(int value)](#setExportCss-int-) | Establece la forma en que se exporta CSS. |
| [setExportFonts(int value)](#setExportFonts-int-) | Establece la forma en que se exportan las fuentes. |
| [setExportImages(int value)](#setExportImages-int-) | Establece la forma en que se exportan las imágenes. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Establece los tipos de fuente. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Establece la devolución de llamada que se invoca para crear el recurso donde almacenar la fuente. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Establece la devolución de llamada que se invoca para crear el recurso donde almacenar la fuente. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Establece un valor que indica si se debe incluir el nombre del proyecto en el encabezado de la página HTML. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Establece un valor que indica si se debe incluir el nombre del proyecto en el título HTML. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Establece una devolución de llamada definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Establece una lista de números de página que se guardarán al renderizar el diseño del proyecto. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Establece un valor que indica si se debe usar un pincel degradado al renderizar el diseño del proyecto. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Inicializa una nueva instancia de la clase [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions).

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
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Obtiene la devolución de llamada que se llama para crear el recurso que almacena CSS.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


Obtiene el prefijo de estilo CSS.

**Returns:**
java.lang.String - prefijo de estilo CSS.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Obtiene la forma en que se exporta CSS.

**Returns:**
int - la forma en que se exportan los CSS.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Obtiene la forma en que se exportan las fuentes.

**Returns:**
int - la forma en que se exportan las fuentes.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Obtiene la forma en que se exportan las imágenes.

**Returns:**
int - la forma en que se exportan las imágenes.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Obtiene los tipos de fuentes.

Valor: Los tipos de fuente.

**Returns:**
int - los tipos de fuente.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Obtiene la devolución de llamada que se llama para crear el recurso que almacena la fuente.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Especifica la configuración de fuentes utilizada al renderizar la vista del proyecto.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Obtiene la devolución de llamada que se llama para crear el recurso que almacena la fuente.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Obtiene un valor que indica si se debe incluir el nombre del proyecto en el encabezado de la página HTML.

**Returns:**
boolean - un valor que indica si se debe incluir el nombre del proyecto en el encabezado de la página HTML.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Obtiene un valor que indica si se debe incluir el nombre del proyecto en el título HTML.

**Returns:**
boolean - un valor que indica si se debe incluir el nombre del proyecto en el título HTML.
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


Obtiene una lista de números de página para guardar al renderizar el diseño del proyecto.

--------------------

Todas las páginas del proyecto se guardarán si esta lista está vacía.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - una lista de números de página que se guardarán al renderizar el diseño del proyecto.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Obtiene un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

**Returns:**
boolean - un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Obtiene un valor que indica si se debe usar un pincel degradado al renderizar el diseño del proyecto.

--------------------

Actualmente, el uso de pincel degradado no es compatible al renderizar a HTML.

**Returns:**
boolean - un valor que indica si se debe usar un pincel degradado al renderizar el diseño del proyecto.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Establece la devolución de llamada que se llama para crear el recurso que almacena CSS.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | la devolución de llamada que se invoca para crear el recurso donde almacenar CSS. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


Establece el prefijo de estilo CSS.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | Prefijo de estilo CSS. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Establece la forma en que se exporta CSS.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la forma en que se exportan los CSS. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Establece la forma en que se exportan las fuentes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la forma en que se exportan las fuentes. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Establece la forma en que se exportan las imágenes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la forma en que se exportan las imágenes. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Establece los tipos de fuente.

Valor: Los tipos de fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | los tipos de fuente. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Establece la devolución de llamada que se invoca para crear el recurso donde almacenar la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | la devolución de llamada que se invoca para crear el recurso que almacena la fuente. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Establece la devolución de llamada que se invoca para crear el recurso donde almacenar la fuente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | la devolución de llamada que se invoca para crear el recurso que almacena la fuente. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Establece un valor que indica si se debe incluir el nombre del proyecto en el encabezado de la página HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe incluir el nombre del proyecto en el encabezado de la página HTML. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Establece un valor que indica si se debe incluir el nombre del proyecto en el título HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe incluir el nombre del proyecto en el título HTML. |

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


Establece una lista de números de página que se guardarán al renderizar el diseño del proyecto.

--------------------

Todas las páginas del proyecto se guardarán si esta lista está vacía.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.List&lt;java.lang.Integer&gt; | una lista de números de página para guardar al renderizar el diseño del proyecto. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Establece un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe reducir el espacio entre la última tarea y el pie de página. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Establece un valor que indica si se debe usar un pincel degradado al renderizar el diseño del proyecto.

--------------------

Actualmente, el uso de pincel degradado no es compatible al renderizar a HTML.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe usar un pincel degradado al renderizar el diseño del proyecto. |

