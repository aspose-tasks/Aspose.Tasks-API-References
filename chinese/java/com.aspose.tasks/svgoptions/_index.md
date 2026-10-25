---
title: "SvgOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目页面渲染为 SVG 时指定其他选项。"
type: docs
weight: 283
url: /zh/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

允许在将项目页面渲染为 SVG 时指定其他选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | 初始化一个新的 [SvgOptions](../../com.aspose/tasks/svgoptions) 类实例，可用于将项目保存为 SVG 格式。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | 获取用户定义的实现回调，用于为每个渲染页面获取输出流。 |
| [getUseGradientBrush()](#getUseGradientBrush--) | 确定在渲染项目布局时是否使用渐变画刷。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 设置用户定义的实现回调，用于为每个渲染页面获取输出流。 |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | 确定在渲染项目布局时是否使用渐变画刷。 |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


初始化一个新的 [SvgOptions](../../com.aspose/tasks/svgoptions) 类实例，可用于将项目保存为 SVG 格式。

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
public final SaveOptions deepClone()
```


保留供内部使用。

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


获取用户定义的实现回调，用于为每个渲染页面获取输出流。

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


确定在渲染项目布局时是否使用渐变画刷。

--------------------

当前不支持在渲染为 SVG 时使用渐变画刷。

**Returns:**
boolean - 指示在渲染项目布局时是否使用渐变画刷的值。
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


设置用户定义的实现回调，用于为每个渲染页面获取输出流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | 用户定义的实现回调，用于为每个渲染页面获取输出流。 |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


确定在渲染项目布局时是否使用渐变画刷。

--------------------

当前不支持在渲染为 SVG 时使用渐变画刷。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示在渲染项目布局时是否使用渐变画刷的值。 |

