---
title: "ParseErrorArgs"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "デリゲートにデータを提供します。"
type: docs
weight: 184
url: /ja/java/com.aspose.tasks/parseerrorargs/
---

**Inheritance:**
java.lang.Object
```
public class ParseErrorArgs
```

デリゲート [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) にデータを提供します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getException()](#getException--) | 文字列値の解析中に発生した例外を取得します。 |
| [getFieldClass()](#getFieldClass--) | オブジェクトフィールドのクラスです。 |
| [getFieldName()](#getFieldName--) | オブジェクトフィールド名を取得します。 |
| [getInvalidValue()](#getInvalidValue--) | 例外を発生させた文字列値を取得します。 |
### getException() {#getException--}
```
public final RuntimeException getException()
```


文字列値の解析中に発生した例外を取得します。

**Returns:**
java.lang.RuntimeException - 文字列値の解析中に発生した例外です。
### getFieldClass() {#getFieldClass--}
```
public Class getFieldClass()
```


オブジェクトフィールドのクラスです。

**Returns:**
java.lang.Class - オブジェクトフィールドのクラスを返します。
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


オブジェクトフィールド名を取得します。

**Returns:**
java.lang.String - オブジェクトフィールド名です。
### getInvalidValue() {#getInvalidValue--}
```
public final String getInvalidValue()
```


例外を発生させた文字列値を取得します。

**Returns:**
java.lang.String - 例外を発生させた文字列値です。
