---
title: XpsOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when rendering project pages to XPS.
type: docs
weight: 366
url: /java/com.aspose.tasks/xpsoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class XpsOptions extends SaveOptions implements ICloneableSaveOptions
```

Allows to specify additional options when rendering project pages to XPS.
## Constructors

| Constructor | Description |
| --- | --- |
| [XpsOptions()](#XpsOptions--) | Initializes a new instance of the [XpsOptions](../../com.aspose.tasks/xpsoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getRenderMetafileAsBitmap()](#getRenderMetafileAsBitmap--) | Gets a value indicating whether a metafile should be rendered as bitmap. |
| [setRenderMetafileAsBitmap(boolean value)](#setRenderMetafileAsBitmap-boolean-) | Sets a value indicating whether a metafile should be rendered as bitmap. |
### XpsOptions() {#XpsOptions--}
```
public XpsOptions()
```


Initializes a new instance of the [XpsOptions](../../com.aspose.tasks/xpsoptions) class.

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
### getRenderMetafileAsBitmap() {#getRenderMetafileAsBitmap--}
```
public final boolean getRenderMetafileAsBitmap()
```


Gets a value indicating whether a metafile should be rendered as bitmap.

**Returns:**
boolean - a value indicating whether a metafile should be rendered as bitmap.
### setRenderMetafileAsBitmap(boolean value) {#setRenderMetafileAsBitmap-boolean-}
```
public final void setRenderMetafileAsBitmap(boolean value)
```


Sets a value indicating whether a metafile should be rendered as bitmap.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether a metafile should be rendered as bitmap. |

