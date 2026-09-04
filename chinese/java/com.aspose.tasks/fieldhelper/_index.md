---
title: "FieldHelper"
second_title: "Aspose.Tasks for Java API 参考"
description: "提供字段实用操作的辅助类。"
type: docs
weight: 88
url: /zh/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

提供字段实用操作的辅助类。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | 返回特定字段的默认标题。 |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | 返回特定任务字段的默认标题。 |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


返回特定字段的默认标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 字段 | int | 用于获取默认标题的字段。 |

**Returns:**
java.lang.String - 如果该字段可以在 MS Project 的视图中显示，则返回特定字段的默认标题；否则返回 null。
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


返回特定任务字段的默认标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| taskKey | 字节 | 用于获取默认标题的任务字段。 |

**Returns:**
java.lang.String - 如果该任务字段可以在 MS Project 的视图中显示，则返回特定任务字段的默认标题；否则返回 null。
