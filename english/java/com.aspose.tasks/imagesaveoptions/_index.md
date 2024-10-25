---
title: ImageSaveOptions
second_title: Aspose.Tasks for Java API Reference
description: Allows to specify additional options when rendering project pages to images.
type: docs
weight: 133
url: /java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Allows to specify additional options when rendering project pages to images.
## Constructors

| Constructor | Description |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Initializes a new instance of the [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) class which can be used to save rendered images in TIFF, PNG, BMP or JPEG formats. |
## Methods

| Method | Description |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | Specifies font settings used when rendering project's view. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Gets the horizontal resolution in dpi. |
| [getJpegQuality()](#getJpegQuality--) | Gets a JPEG quality. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Gets a user-defined callback which is used to get an output stream for each rendered page. |
| [getPages()](#getPages--) | Gets a list of page numbers to save when saving project layout to separate files. |
| [getPixelFormat()](#getPixelFormat--) | Gets the format of the color data for each pixel in the image. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Gets a value indicating whether a gap between last task and the footer must be reduced. |
| [getTiffCompression()](#getTiffCompression--) | Gets the type of compression to apply when saving generated images to the TIFF format. |
| [getVerticalResolution()](#getVerticalResolution--) | Gets the vertical resolution in dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Sets the horizontal resolution in dpi. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Sets a JPEG quality. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Sets a user-defined callback which is used to get an output stream for each rendered page. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Sets a list of page numbers to save when saving project layout to separate files. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Sets the format of the color data for each pixel in the image. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Sets a value indicating whether a gap between last task and the footer must be reduced. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Sets the type of compression to apply when saving generated images to the TIFF format. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Sets the vertical resolution in dpi. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Initializes a new instance of the [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) class which can be used to save rendered images in TIFF, PNG, BMP or JPEG formats.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | Can be TIFF, PNG, BMP or JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat). |

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
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Specifies font settings used when rendering project's view.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Gets the horizontal resolution in dpi.

**Returns:**
float - the horizontal resolution in dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Gets a JPEG quality. The allowed value range is 0..100.

**Returns:**
int - a JPEG quality.
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


Gets a list of page numbers to save when saving project layout to separate files.

--------------------

All pages will be saved if this list is empty.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - a list of page numbers to save when saving project layout to separate files.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Gets the format of the color data for each pixel in the image.

**Returns:**
int - the format of the color data for each pixel in the image.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Gets a value indicating whether a gap between last task and the footer must be reduced.

**Returns:**
boolean - a value indicating whether a gap between last task and the footer must be reduced.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Gets the type of compression to apply when saving generated images to the TIFF format.

--------------------

Has effect only when saving to TIFF. The default value is `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - the type of compression to apply when saving generated images to the TIFF format.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Gets the vertical resolution in dpi.

**Returns:**
float - the vertical resolution in dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Sets the horizontal resolution in dpi.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | the horizontal resolution in dpi. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Sets a JPEG quality. The allowed value range is 0..100.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a JPEG quality. |

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


Sets a list of page numbers to save when saving project layout to separate files.

--------------------

All pages will be saved if this list is empty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;java.lang.Integer&gt; | a list of page numbers to save when saving project layout to separate files. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Sets the format of the color data for each pixel in the image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the format of the color data for each pixel in the image. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Sets a value indicating whether a gap between last task and the footer must be reduced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether a gap between last task and the footer must be reduced. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Sets the type of compression to apply when saving generated images to the TIFF format.

--------------------

Has effect only when saving to TIFF. The default value is `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the type of compression to apply when saving generated images to the TIFF format. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Sets the vertical resolution in dpi.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float | the vertical resolution in dpi. |

