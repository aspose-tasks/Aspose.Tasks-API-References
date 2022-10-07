---
title: FontResolveEventArgs
second_title: Aspose.Tasks for Java API Reference
description: Provides arguments for the callback that is invoked when font is resolved.
type: docs
weight: 99
url: /java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Provides arguments for the callback that is invoked when font is resolved.
## Methods

| Method | Description |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | Gets the name of requested font. |
| [getResolvedFontName()](#getResolvedFontName--) | Gets the name of resolved font. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Sets the name of resolved font. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


Gets the name of requested font.

**Returns:**
java.lang.String - the name of requested font.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Gets the name of resolved font. Can be set to control fonts used to render a view.

**Returns:**
java.lang.String - Name of the requested font if font is found or name of fallback font or null if font cannot be found.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Sets the name of resolved font. Can be set to control fonts used to render a view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of resolved font. |

