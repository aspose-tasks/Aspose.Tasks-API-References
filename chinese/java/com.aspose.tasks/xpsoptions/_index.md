---
title: "XpsOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目页面渲染为 XPS 时指定附加选项。"
type: docs
weight: 369
url: /zh/java/com.aspose.tasks/xpsoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class XpsOptions extends SaveOptions implements ICloneableSaveOptions
```

允许在将项目页面渲染为 XPS 时指定附加选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [XpsOptions()](#XpsOptions--) | 初始化 [XpsOptions](../../com.aspose.tasks/xpsoptions) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getRenderMetafileAsBitmap()](#getRenderMetafileAsBitmap--) | 获取一个值，指示是否应将元文件渲染为位图。 |
| [setRenderMetafileAsBitmap(boolean value)](#setRenderMetafileAsBitmap-boolean-) | 设置一个值，指示是否应将元文件渲染为位图。 |
### XpsOptions() {#XpsOptions--}
```
public XpsOptions()
```


初始化 [XpsOptions](../../com.aspose.tasks/xpsoptions) 类的新实例。

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
### getRenderMetafileAsBitmap() {#getRenderMetafileAsBitmap--}
```
public final boolean getRenderMetafileAsBitmap()
```


获取一个值，指示是否应将元文件渲染为位图。

**Returns:**
boolean - 一个指示是否应将元文件渲染为位图的值。
### setRenderMetafileAsBitmap(boolean value) {#setRenderMetafileAsBitmap-boolean-}
```
public final void setRenderMetafileAsBitmap(boolean value)
```


设置一个值，指示是否应将元文件渲染为位图。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个指示是否应将元文件渲染为位图的值。 |

