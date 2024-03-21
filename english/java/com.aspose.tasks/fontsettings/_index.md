---
title: FontSettings
second_title: Aspose.Tasks for Java API Reference
description: Specifies font settings used when rendering projects view.
type: docs
weight: 101
url: /java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Specifies font settings used when rendering project's view.
## Constructors

| Constructor | Description |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | Gets the default (or fallback) font for rendering. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Gets a callback which can be used to customize resolved fonts. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Gets a value indicating whether the default font must be used for rendering. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Sets the default (or fallback) font for rendering. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Sets the folders where Aspose.Tasks looks for TrueType fonts when rendering project's view. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Sets a callback which can be used to customize resolved fonts. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Sets a value indicating whether the default font must be used for rendering. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Gets the default (or fallback) font for rendering.

**Returns:**
java.lang.String - the default (or fallback) font for rendering.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Gets a callback which can be used to customize resolved fonts.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Gets a value indicating whether the default font must be used for rendering.

--------------------

When the value is False and DefaultFontName is specified, the rendering engine will utilize the font specified by DefaultFontName as a fallback font. Otherwise 'Arial' (if installed) or 'Generic Sans Serif' fonts are used as a fallback font. The fallback font is utilized during the rendering of project view when a text style references a font that is not installed on the current operating system. For greater control over font resolution you can use `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Returns:**
boolean - a value indicating whether the default font must be used for rendering.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Sets the default (or fallback) font for rendering.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the default (or fallback) font for rendering. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Sets the folders where Aspose.Tasks looks for TrueType fonts when rendering project's view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | java.lang.String[] | An array of folders that contain TrueType fonts. |
| recursive | boolean | If true the specified folders will be scanned recursively. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Sets a callback which can be used to customize resolved fonts.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | a callback which can be used to customize resolved fonts. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Sets a value indicating whether the default font must be used for rendering.

--------------------

When the value is False and DefaultFontName is specified, the rendering engine will utilize the font specified by DefaultFontName as a fallback font. Otherwise 'Arial' (if installed) or 'Generic Sans Serif' fonts are used as a fallback font. The fallback font is utilized during the rendering of project view when a text style references a font that is not installed on the current operating system. For greater control over font resolution you can use `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the default font must be used for rendering. |

