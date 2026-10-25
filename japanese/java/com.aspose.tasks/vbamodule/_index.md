---
title: "VbaModule"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "VBAモジュールを表します。"
type: docs
weight: 334
url: /ja/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

VBAモジュールを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | [VbaModule](../../com.aspose/tasks/vbamodule) のインスタンスを VbaModuleType.ClassModule タイプで作成します。 |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | [VbaModule](../../com.aspose/tasks/vbamodule) のインスタンスを作成し、VbaModuleType.ProceduralModule タイプを使用します。 |
| [getAttributes()](#getAttributes--) | モジュールの属性コレクションを取得します。 |
| [getName()](#getName--) | VBA モジュールの名前を取得します |
| [getSourceCode()](#getSourceCode--) | VBA モジュールのソースコードを取得します |
| [getType()](#getType--) | モジュールのタイプを取得します。 |
| [setName(String value)](#setName-java.lang.String-) | VBA モジュールの名前 |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | VBA モジュールのソースコードを設定します |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


[VbaModule](../../com.aspose/tasks/vbamodule) のインスタンスを VbaModuleType.ClassModule タイプで作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


[VbaModule](../../com.aspose/tasks/vbamodule) のインスタンスを作成し、VbaModuleType.ProceduralModule タイプを使用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


モジュールの属性コレクションを取得します。

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


VBA モジュールの名前を取得します

**Returns:**
java.lang.String - VBA モジュールの名前
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


VBA モジュールのソースコードを取得します

**Returns:**
java.lang.String - VBA モジュールのソースコード
### getType() {#getType--}
```
public final int getType()
```


モジュールのタイプを取得します。

**Returns:**
int - モジュールのタイプです。
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


VBA モジュールの名前

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | VBA モジュールの名前 |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


VBA モジュールのソースコードを設定します

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | VBA モジュールのソースコード |

