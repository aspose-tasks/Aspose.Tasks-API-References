---
title: SvgOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when rendering project pages to SVG.
type: docs
weight: 282
url: /java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Allows to specify additional options when rendering project pages to SVG.
## Constructors

| Constructor | Description |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Initializes a new instance of the [SvgOptions](../../com.aspose.tasks/svgoptions) class that can be used to save project in SVG format. |
## Methods

| Method | Description |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Gets a user-defined implementation callback which is used to get an output stream for each rendered page. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Determines whether to use gradient brush when rendering project layout. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Sets a user-defined implementation callback which is used to get an output stream for each rendered page. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Determines whether to use gradient brush when rendering project layout. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Initializes a new instance of the [SvgOptions](../../com.aspose.tasks/svgoptions) class that can be used to save project in SVG format.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Reserved for internal usage.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public final SaveOptions deepClone()
```


Reserved for internal usage.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Gets a user-defined implementation callback which is used to get an output stream for each rendered page.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Determines whether to use gradient brush when rendering project layout.

--------------------

Currently using of gradient brush is not supported for rendering to SVG.

**Returns:**
boolean - value indicating whether to use gradient brush when rendering project layout.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Sets a user-defined implementation callback which is used to get an output stream for each rendered page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | a user-defined implementation callback which is used to get an output stream for each rendered page. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Determines whether to use gradient brush when rendering project layout.

--------------------

Currently using of gradient brush is not supported for rendering to SVG.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | value indicating whether to use gradient brush when rendering project layout. |

