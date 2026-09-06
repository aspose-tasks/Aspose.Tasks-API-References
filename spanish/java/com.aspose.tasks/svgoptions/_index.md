---
title: "SvgOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al renderizar páginas de proyecto a SVG."
type: docs
weight: 283
url: /es/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Permite especificar opciones adicionales al renderizar páginas de proyecto a SVG.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Inicializa una nueva instancia de la clase [SvgOptions](../../com.aspose.tasks/svgoptions) que puede usarse para guardar el proyecto en formato SVG. |
## Métodos

| Método | Descripción |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Obtiene una devolución de llamada de implementación definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Determina si se debe usar un pincel de degradado al renderizar el diseño del proyecto. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Establece una devolución de llamada de implementación definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Determina si se debe usar un pincel de degradado al renderizar el diseño del proyecto. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Inicializa una nueva instancia de la clase [SvgOptions](../../com.aspose.tasks/svgoptions) que puede usarse para guardar el proyecto en formato SVG.

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
public final SaveOptions deepClone()
```


Reservado para uso interno.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Obtiene una devolución de llamada de implementación definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Determina si se debe usar un pincel de degradado al renderizar el diseño del proyecto.

--------------------

Actualmente el uso de pincel de degradado no es compatible para renderizar a SVG.

**Returns:**
boolean - valor que indica si se debe usar un pincel de degradado al renderizar el diseño del proyecto.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Establece una devolución de llamada de implementación definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | una devolución de llamada de implementación definida por el usuario que se utiliza para obtener un flujo de salida para cada página renderizada. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Determina si se debe usar un pincel de degradado al renderizar el diseño del proyecto.

--------------------

Actualmente el uso de pincel de degradado no es compatible para renderizar a SVG.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | valor que indica si se debe usar un pincel de degradado al renderizar el diseño del proyecto. |

