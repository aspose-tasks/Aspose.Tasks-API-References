---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目页面渲染为 PDF 时指定附加选项。"
type: docs
weight: 191
url: /zh/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

允许在将项目页面渲染为 PDF 时指定附加选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | 初始化一个新的 [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) 类实例，可用于将文档保存为 [SaveFileFormat](../../com.aspose.tasks/savefileformat) 格式。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | 获取生成的 PDF 文档的所需合规级别。 |
| [getEncryptionDetails()](#getEncryptionDetails--) | 获取加密详细信息。 |
| [getFontSettings()](#getFontSettings--) | 指定在渲染项目视图时使用的字体设置。 |
| [getPageSavingCallback()](#getPageSavingCallback--) | 获取用户定义的回调，用于为每个渲染的页面获取输出流。 |
| [getPages()](#getPages--) | 获取在将项目布局保存为单独文件时要保存的页码列表。 |
| [getReduceFooterGap()](#getReduceFooterGap--) | 获取指示是否必须缩小最后任务与页脚之间间距的值。 |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | 获取指示是否将项目页面保存为单独文件的值。 |
| [getTextCompression()](#getTextCompression--) | 获取用于除图像之外的所有内容流的压缩类型。 |
| [setCompliance(int value)](#setCompliance-int-) | 设置生成的 PDF 文档的所需合规级别。 |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | 设置加密详细信息。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 设置用户定义的回调函数，用于获取每个渲染页面的输出流。 |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | 设置在将项目布局保存为单独文件时要保存的页码列表。 |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | 设置一个值，指示是否必须缩小最后任务与页脚之间的间距。 |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | 设置指示是否将项目页面保存为单独文件的值。 |
| [setTextCompression(int value)](#setTextCompression-int-) | 设置用于除图像之外的所有内容流的压缩类型。 |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


初始化一个新的 [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) 类实例，可用于将文档保存为 [SaveFileFormat](../../com.aspose.tasks/savefileformat) 格式。

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
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
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


获取生成的 PDF 文档的所需合规级别。默认值为 [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15)。

**Returns:**
int - 生成的 PDF 文档的所需合规级别。
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


获取加密详细信息。如果未设置，则不会执行加密。

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


指定在渲染项目视图时使用的字体设置。

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


获取用于为每个渲染页面获取输出流的用户定义回调。当使用 `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) 选项时适用。

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


获取在将项目布局保存为单独文件时要保存的页码列表。

--------------------

如果此列表为空，将保存所有页面。

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - 在将项目布局保存为单独文件时要保存的页码列表。
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


获取指示是否必须缩小最后任务与页脚之间间距的值。

**Returns:**
boolean - 一个值，指示是否必须缩小最后任务与页脚之间的间距。
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


获取指示是否将项目页面保存为单独文件的值。

**Returns:**
boolean - 指示是否将项目页面保存为单独文件的值。
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


获取用于除图像之外的所有内容流的压缩类型。默认值为 [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate)。

**Returns:**
int - 用于除图像之外的所有内容流的压缩类型。
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


设置生成的 PDF 文档的所需合规级别。默认值为 [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 生成的 PDF 文档的所需合规级别。 |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


设置加密详细信息。如果未设置，则不会执行加密。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | 加密详细信息。 |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


设置用于为每个渲染页面获取输出流的用户定义回调。当使用 `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) 选项时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | 用户定义的回调，用于获取每个渲染页面的输出流。 |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


设置在将项目布局保存为单独文件时要保存的页码列表。

--------------------

如果此列表为空，将保存所有页面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.List&lt;java.lang.Integer&gt; | 在将项目布局保存为单独文件时要保存的页码列表。 |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


设置一个值，指示是否必须缩小最后任务与页脚之间的间距。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否应缩小最后任务与页脚之间间距的值。 |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


设置指示是否将项目页面保存为单独文件的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个指示是否将项目页面保存为单独文件的值。 |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


设置用于除图像之外的所有内容流的压缩类型。默认是 [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 用于除图像之外的所有内容流的压缩类型。 |

