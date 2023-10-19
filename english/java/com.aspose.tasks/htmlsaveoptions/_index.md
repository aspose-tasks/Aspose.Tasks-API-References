---
title: HtmlSaveOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when rendering project pages to HTML.
type: docs
weight: 127
url: /java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Allows to specify additional options when rendering project pages to HTML.
## Constructors

| Constructor | Description |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Initializes a new instance of the [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | Gets the callback that is called to create resource to store CSS. |
| [getCssStylePrefix()](#getCssStylePrefix--) | Gets CSS style prefix. |
| [getDefaultFontName()](#getDefaultFontName--) | Gets the default (or fallback) font for rendering. |
| [getExportCss()](#getExportCss--) | Gets the way CSS are exported. |
| [getExportFonts()](#getExportFonts--) | Gets the way fonts are exported. |
| [getExportImages()](#getExportImages--) | Gets the way images are exported. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Gets the font face types. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Gets a callback which can be used to customize resolved fonts. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Gets the callback that is called to create resource to store font. |
| [getFontSettings()](#getFontSettings--) | Specifies font settings used when rendering project's view. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Gets the callback that is called to create resource to store font. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Gets a value indicating whether to include project name in HTML page header. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Gets a value indicating whether to include project name in HTML title. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Gets a user-defined callback which is used to get an output stream for each rendered page. |
| [getPages()](#getPages--) | Gets a list of page numbers to save when rendering project layout. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Gets a value indicating whether a gap between last task and the footer must be reduced. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Gets a value indicating whether to use gradient brush when rendering project layout. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Gets a value indicating whether the default font must be used for rendering. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | Sets the callback that is called to create resource to store CSS. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | Sets CSS style prefix. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Sets the default (or fallback) font for rendering. |
| [setExportCss(int value)](#setExportCss-int-) | Sets the way CSS are exported. |
| [setExportFonts(int value)](#setExportFonts-int-) | Sets the way fonts are exported. |
| [setExportImages(int value)](#setExportImages-int-) | Sets the way images are exported. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Sets the font face types. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Sets a callback which can be used to customize resolved fonts. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Sets the callback that is called to create resource to store font. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Sets the callback that is called to create resource to store font. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Sets a value indicating whether to include project name in HTML page header. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Sets a value indicating whether to include project name in HTML title. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Sets a user-defined callback which is used to get an output stream for each rendered page. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Sets a list of page numbers to save when rendering project layout. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Sets a value indicating whether a gap between last task and the footer must be reduced. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Sets a value indicating whether to use gradient brush when rendering project layout. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Sets a value indicating whether the default font must be used for rendering. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Initializes a new instance of the [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) class.

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
public SaveOptions deepClone()
```


Reserved for internal usage.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Gets the callback that is called to create resource to store CSS.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


Gets CSS style prefix.

**Returns:**
java.lang.String - CSS style prefix.
### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Gets the default (or fallback) font for rendering.

**Returns:**
java.lang.String - the default (or fallback) font for rendering.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Gets the way CSS are exported.

**Returns:**
int - the way CSS are exported.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Gets the way fonts are exported.

**Returns:**
int - the way fonts are exported.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Gets the way images are exported.

**Returns:**
int - the way images are exported.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Gets the font face types.

Value: The font face types.

**Returns:**
int - the font face types.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Gets a callback which can be used to customize resolved fonts.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Gets the callback that is called to create resource to store font.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Specifies font settings used when rendering project's view.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Gets the callback that is called to create resource to store font.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Gets a value indicating whether to include project name in HTML page header.

**Returns:**
boolean - a value indicating whether to include project name in HTML page header.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Gets a value indicating whether to include project name in HTML title.

**Returns:**
boolean - a value indicating whether to include project name in HTML title.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Gets a user-defined callback which is used to get an output stream for each rendered page.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Gets a list of page numbers to save when rendering project layout.

--------------------

All project pages will be saved if this list is empty.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - a list of page numbers to save when rendering project layout.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Gets a value indicating whether a gap between last task and the footer must be reduced.

**Returns:**
boolean - a value indicating whether a gap between last task and the footer must be reduced.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Gets a value indicating whether to use gradient brush when rendering project layout.

--------------------

Currently using of gradient brush is not supported when rendering to HTML.

**Returns:**
boolean - a value indicating whether to use gradient brush when rendering project layout.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Gets a value indicating whether the default font must be used for rendering.

--------------------

When the value is False and DefaultFontName is specified, the rendering engine will utilize the font specified by DefaultFontName as a fallback font. Otherwise 'Arial' (if installed) or 'Generic Sans Serif' fonts are used as a fallback font. The fallback font is utilized during the rendering of project view when a text style references a font that is not installed on the current operating system. For greater control over font resolution you can use  FontResolveCallback ([getFontResolveCallback](../../com.aspose.tasks/htmlsaveoptions\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/htmlsaveoptions\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Returns:**
boolean - a value indicating whether the default font must be used for rendering.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Sets the callback that is called to create resource to store CSS.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | the callback that is called to create resource to store CSS. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


Sets CSS style prefix.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | CSS style prefix. |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Sets the default (or fallback) font for rendering.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the default (or fallback) font for rendering. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Sets the way CSS are exported.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the way CSS are exported. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Sets the way fonts are exported.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the way fonts are exported. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Sets the way images are exported.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the way images are exported. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Sets the font face types.

Value: The font face types.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the font face types. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Sets a callback which can be used to customize resolved fonts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | a callback which can be used to customize resolved fonts. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Sets the callback that is called to create resource to store font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | the callback that is called to create resource to store font. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Sets the callback that is called to create resource to store font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | the callback that is called to create resource to store font. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Sets a value indicating whether to include project name in HTML page header.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to include project name in HTML page header. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Sets a value indicating whether to include project name in HTML title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to include project name in HTML title. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Sets a user-defined callback which is used to get an output stream for each rendered page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | a user-defined callback which is used to get an output stream for each rendered page. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Sets a list of page numbers to save when rendering project layout.

--------------------

All project pages will be saved if this list is empty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;java.lang.Integer&gt; | a list of page numbers to save when rendering project layout. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Sets a value indicating whether a gap between last task and the footer must be reduced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether a gap between last task and the footer must be reduced. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Sets a value indicating whether to use gradient brush when rendering project layout.

--------------------

Currently using of gradient brush is not supported when rendering to HTML.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to use gradient brush when rendering project layout. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Sets a value indicating whether the default font must be used for rendering.

--------------------

When the value is False and DefaultFontName is specified, the rendering engine will utilize the font specified by DefaultFontName as a fallback font. Otherwise 'Arial' (if installed) or 'Generic Sans Serif' fonts are used as a fallback font. The fallback font is utilized during the rendering of project view when a text style references a font that is not installed on the current operating system. For greater control over font resolution you can use  FontResolveCallback ([getFontResolveCallback](../../com.aspose.tasks/htmlsaveoptions\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/htmlsaveoptions\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the default font must be used for rendering. |

