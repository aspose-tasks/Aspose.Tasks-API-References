---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目页面渲染为 HTML 时指定其他选项。"
type: docs
weight: 132
url: /zh/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

允许在将项目页面渲染为 HTML 时指定其他选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | 初始化 [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | 获取用于创建存储 CSS 资源的回调。 |
| [getCssStylePrefix()](#getCssStylePrefix--) | 获取 CSS 样式前缀。 |
| [getExportCss()](#getExportCss--) | 获取 CSS 的导出方式。 |
| [getExportFonts()](#getExportFonts--) | 获取字体的导出方式。 |
| [getExportImages()](#getExportImages--) | 获取图像的导出方式。 |
| [getFontFaceTypes()](#getFontFaceTypes--) | 获取字体面类型。 |
| [getFontSavingCallback()](#getFontSavingCallback--) | 获取用于创建存储字体资源的回调。 |
| [getFontSettings()](#getFontSettings--) | 指定在渲染项目视图时使用的字体设置。 |
| [getImageSavingCallback()](#getImageSavingCallback--) | 获取用于创建存储字体资源的回调。 |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | 获取指示是否在 HTML 页面页眉中包含项目名称的值。 |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | 获取指示是否在 HTML 标题中包含项目名称的值。 |
| [getPageSavingCallback()](#getPageSavingCallback--) | 获取用户定义的回调，用于为每个渲染的页面获取输出流。 |
| [getPages()](#getPages--) | 获取在渲染项目布局时要保存的页码列表。 |
| [getReduceFooterGap()](#getReduceFooterGap--) | 获取指示是否必须缩小最后任务与页脚之间间距的值。 |
| [getUseGradientBrush()](#getUseGradientBrush--) | 获取指示在渲染项目布局时是否使用渐变画笔的值。 |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | 设置用于创建存储 CSS 资源的回调。 |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | 设置 CSS 样式前缀。 |
| [setExportCss(int value)](#setExportCss-int-) | 设置 CSS 的导出方式。 |
| [setExportFonts(int value)](#setExportFonts-int-) | 设置字体的导出方式。 |
| [setExportImages(int value)](#setExportImages-int-) | 设置图像的导出方式。 |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | 设置字体族类型。 |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | 设置用于创建存储字体资源的回调函数。 |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | 设置用于创建存储字体资源的回调函数。 |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | 设置一个值，指示是否在 HTML 页面标题栏中包含项目名称。 |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | 设置一个值，指示是否在 HTML 标题中包含项目名称。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 设置用户定义的回调函数，用于获取每个渲染页面的输出流。 |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | 设置在渲染项目布局时要保存的页码列表。 |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | 设置一个值，指示是否必须缩小最后任务与页脚之间的间距。 |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | 设置一个值，指示在渲染项目布局时是否使用渐变画刷。 |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


初始化 [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) 类的新实例。

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


保留供内部使用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


保留供内部使用。

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


获取用于创建存储 CSS 资源的回调。

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


获取 CSS 样式前缀。

**Returns:**
java.lang.String - CSS 样式前缀。
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


获取 CSS 的导出方式。

**Returns:**
int - CSS 的导出方式。
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


获取字体的导出方式。

**Returns:**
int - 字体的导出方式。
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


获取图像的导出方式。

**Returns:**
int - 图像的导出方式。
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


获取字体面类型。

值：字体族类型。

**Returns:**
int - 字体族类型。
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


获取用于创建存储字体资源的回调。

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


指定在渲染项目视图时使用的字体设置。

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


获取用于创建存储字体资源的回调。

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


获取指示是否在 HTML 页面页眉中包含项目名称的值。

**Returns:**
boolean - 一个值，指示是否在 HTML 页面标题栏中包含项目名称。
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


获取指示是否在 HTML 标题中包含项目名称的值。

**Returns:**
boolean - 一个值，指示是否在 HTML 标题中包含项目名称。
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


获取用户定义的回调，用于为每个渲染的页面获取输出流。

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


获取在渲染项目布局时要保存的页码列表。

--------------------

如果此列表为空，将保存所有项目页面。

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - 在渲染项目布局时要保存的页码列表。
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


获取指示是否必须缩小最后任务与页脚之间间距的值。

**Returns:**
boolean - 一个值，指示是否必须缩小最后任务与页脚之间的间距。
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


获取指示在渲染项目布局时是否使用渐变画笔的值。

--------------------

当前在渲染为 HTML 时不支持使用渐变画刷。

**Returns:**
boolean - 一个值，指示在渲染项目布局时是否使用渐变画刷。
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


设置用于创建存储 CSS 资源的回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | 用于创建存储 CSS 资源的回调函数。 |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


设置 CSS 样式前缀。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | CSS 样式前缀。 |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


设置 CSS 的导出方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | CSS 导出的方式。 |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


设置字体的导出方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 字体导出的方式。 |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


设置图像的导出方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 图像导出的方式。 |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


设置字体族类型。

值：字体族类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 字体面类型。 |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


设置用于创建存储字体资源的回调函数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | 用于创建存储字体资源的回调。 |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


设置用于创建存储字体资源的回调函数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | 用于创建存储字体资源的回调。 |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


设置一个值，指示是否在 HTML 页面标题栏中包含项目名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否在 HTML 页面头部包含项目名称的值。 |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


设置一个值，指示是否在 HTML 标题中包含项目名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否在 HTML 标题中包含项目名称的值。 |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


设置用户定义的回调函数，用于获取每个渲染页面的输出流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | 用户定义的回调，用于获取每个渲染页面的输出流。 |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


设置在渲染项目布局时要保存的页码列表。

--------------------

如果此列表为空，将保存所有项目页面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.List&lt;java.lang.Integer&gt; | 在渲染项目布局时要保存的页码列表。 |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


设置一个值，指示是否必须缩小最后任务与页脚之间的间距。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否应缩小最后任务与页脚之间间距的值。 |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


设置一个值，指示在渲染项目布局时是否使用渐变画刷。

--------------------

当前在渲染为 HTML 时不支持使用渐变画刷。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示在渲染项目布局时是否使用渐变画刷的值。 |

